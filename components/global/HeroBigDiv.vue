<template>
    <div>
        <div class="hero-big-div">
            <h1>{{ heroBigDiv.title }}</h1>
            <div class="sm-container">
                <!-- <HeroTwoSmDivs /> -->
                <HeroSmDiv />
            </div>
        </div>
    </div>
</template>

<script>
import HeroSmDiv from './HeroSmDiv.vue'

export default {
    props: {
        heroBigDiv: {
            type: Object,
            required: true
        }
    }, 
    components: true
}
</script>

<style>
    .hero-big-div {
        margin: 25px;
        width: 700px;
        height: 500px;
        background: black;
        color: white;
        text-align: center;
        display: flex;
        flex-direction: column;
        justify-content: end;
        align-items: center;
        border-radius: 5px; 
    }

    .sm-container {
        background: white;
        height: 200px;
        width: 500px;
        position: relative;
        top: 100px;
        box-shadow: 1px 1px 10px 1px gray;
        border-radius: 5px; 
        display: flex;
        flex-direction: column;
        justify-content: center;
    }
</style>