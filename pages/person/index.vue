<template>
  <div class="people-container">
    <h1>people</h1>
    <ul>
      <li v-for="person of people" :key="person.slug">
       <NuxtLink :to="{ name: 'person-slug', params: { slug: person.slug } }">          
         <div>
              <h2>{{ person.name }}</h2>
              <p>{{ person.occupation }}</p>
              <p>{{ person.age }}</p>
          </div>
        </NuxtLink>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
    async asyncData({ $content, params }) {
      const people = await $content('people')
        .only(['name', 'occupation', 'age', 'slug'])
        .fetch()

      return {
        people
      }
    }
}
</script>

<style>

</style>