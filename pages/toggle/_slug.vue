<template>
    <div>
        <nuxt-content :document="page" />
    </div>
</template>

<script>
export default {
    async asyncData({ $content, params }) {
      const page = await $content('toggle', params.slug).fetch()
      return { page }
    }
}
</script>