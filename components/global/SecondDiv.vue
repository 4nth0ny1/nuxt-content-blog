<template>
  <div>
      <div>
          <h1>{{ toggleDivs.christmas }}</h1>
      </div>
  </div>
</template>

<script>
export default {
    props: {
        toggleDivs: {
            type: Object,
            required: true
        }
    }
}
</script>

<style>

</style>