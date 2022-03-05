<template>
<header>
  <div class="hero-container"></div>
  <div class="home-container">
    <div class="second-section">
      <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.</p>
    </div>

    <div class="third-section">
      <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.</p>
    </div>

    <div class="card-section">
      <div class="card">
        <img src="https://images.unsplash.com/photo-1533122250115-6bb28e9a48c3?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1035&q=80" alt="">
        <h2>header</h2>
        <p>It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.</p>
      </div>
      <div class="card">
        <img src="https://images.unsplash.com/photo-1579548122080-c35fd6820ecb?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=2340&q=80" alt="">
        <h2>header</h2>
        <p>It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.</p>
      </div>
      <div class="card">
        <img src="https://images.unsplash.com/photo-1570402211808-cfef7aa6e806?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=3570&q=80" alt="">
        <h2>header</h2>
        <p>It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.</p>
      </div>
    </div>
  </div>
  <div class="full-section">
    <div class="full-section-inner">
      <p>Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book.</p>
    </div>
  </div>
</header>
</template> 

<script>
export default {
    name: 'IndexPage'
}
</script>

<style>
  .home-container {
    max-width: 800px;
    margin: 0 auto;
  }

  .hero-container {
    background: black;
    height: 600px;
    color: #eeeeee;
  }

  .home-container h1 {
    text-align: center;
    margin-top: 10px;
  }

  .second-section, 
  .third-section {
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 50px 50px 0px 50px;
    text-align: center;
  }

  .card-section {
    display: flex; 
    flex-direction: column;
    justify-content: center;
    align-items: center;
    margin: 25px;
  }

  .card {
    background: white;
    width: 300px;
    /* border: 1px solid black; */
    border-radius: 10px;
    box-shadow: 1px 1px 7px 0px black;
    margin: 25px;
    padding: 15px;
  }

  .card img {
    width: 100%;
    max-height: 200px;
  }

  .card h2 {
    margin: 10px 0px;
  }

  .full-section {
    display: flex;
    justify-content: center;
    text-align: center;
    margin: 25px;
  }

  .full-section-inner {
    background: black;
    color: white;
    border: 100px solid white;
    border-radius: 50%;
    padding: 50px; 
    width: 450px;
    height: 450px;
    box-shadow: 1px 1px 7px 0px black;
  }



</style>