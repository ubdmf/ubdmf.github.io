<template>
  <div>
    <ul
      class="text-gray-500 max-w-5xl mx-auto px-6 py-6 rounded-xl bg-white/80 dark:bg-gray-600/60 blur-md shadow"
    >
      <li
        v-for="article of articles"
        :key="article.slug"
        class="mb-12 last:mb-0 bg-white dark:bg-slate-800/50 p-5 rounded-md shadow"
      >
        <NuxtLink
          :to="{ name: 'articles-slug', params: { slug: article.slug } }"
          class="md:grid md:gap-4 md:grid-cols-2"
        >
          <img
            :src="article.image || '/imgs/yellow.webp'"
            class="mb-4 border rounded"
          />
          <div>
            <h2
              class="font-bold text-gray-900 dark:text-gray-300 text-2xl mb-2"
            >
              {{ article.title }}
            </h2>
            <p class="text-lg dark:text-gray-400">{{ article.description }}</p>
            <p class="font-bold text-blue-600 dark:text-indigo-400 mt-2">
              查看更多<span class="text-indigo-600 dark:text-indigo-400"
                >&hellip;</span
              >
            </p>
          </div>
        </NuxtLink>
      </li>
    </ul>
    <div v-if="total" class="container mx-auto my-8 max-w-5xl">
      <Pagination v-if="total > 5" :total="total" />
    </div>
  </div>
</template>

<script>
import Pagination from '@/components/Pagination'

export default {
  name: 'ArticleList',
  components: {
    Pagination,
  },
  props: {
    articles: {
      type: Array,
      default: Array,
    },
    total: {
      type: Number,
      default: 0,
    },
  },
}
</script>
