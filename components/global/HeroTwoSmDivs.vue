<template>
  <div class="two-div-sm-container">
      <div class="sm-div-one">
          <h1>left div</h1>
          <h1>left div</h1>
      </div>
      <div class="sm-div-two">
          <h1>right div</h1>
          <h1>right div</h1>
      </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>
    .two-div-sm-container {
        display: flex;
        flex-direction: row; 
        justify-content: space-between;
        color: black;
        height: 100%;
    }

    .sm-div-one, 
    .sm-div-two {
        width: 100%;
        border-left: 1px solid black;
        border-right: 1px solid black;
        display: flex;
        flex-direction: column;
        justify-content: center;
    }



</style>