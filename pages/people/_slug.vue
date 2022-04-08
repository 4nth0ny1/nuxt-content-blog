<template>
    <div>
        <h1>{{ person.name }}</h1>
        <p>{{ person.occupation }}</p>
        <p>{{ person.age }}</p>

        <nuxt-content :document="person" />
    </div>
</template>

<script>
export default {
    async asyncData({ $content, params }) {
      const person = await $content('people', params.slug).fetch()
      return { person }
    },
    async asyncData({ $content, params }) {
      const person = await $content('people', params.slug).fetch()
    
        // await $content('people')
        // .only(['name', 'slug'])
        // .surround(params.slug)
        // .fetch()

        return {
            person
        }
    }
}
</script>

<style>

</style>