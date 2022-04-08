<template>
  <div>
      <h1>Name: {{ name }}</h1>
      <p>Occupation: {{ occupation }}</p>
      <p>Age: {{ age }}</p>
  </div>
</template>

<script>
export default {
    props: {
        name: {
            type: String,
            default: ''
        }, 
        occupation: {
            type: String, 
            default: ''
        }, 
        age: {
            type: Number, 
            default: 0
        }
    }
}
</script>

<style>

</style>