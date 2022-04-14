<template>
    <div>
        <p>{{ toggleDivs.title }}</p>
        <p>{{ toggleDivs.description }}</p>

        <div class="colors">
            <h1 class="blue" v-on:click="e => disabled && toggle()" :class="{ underline: !isActive }">Easter</h1>
            <h1 class="red" v-on:click="e => !disabled && toggle()"  :class="{ underline: isActive }">Christmas</h1>
        </div>

        <div v-if="!isActive" class="div-one">
            <NewDiv :toggleDivs="toggleDivs" />
        </div>

        <div v-if="isActive" class="div-two">
            <SecondDiv :toggleDivs="toggleDivs" />
        </div>
    </div>
</template>

<script>
import NewDiv from "./NewDiv.vue"
import SecondDiv from './SecondDiv.vue'

export default {
    props: {
        toggleDivs: {
            type: Object,
            required: true
        }
    },
    data() {
        return {
            isActive: false,
            disabled: false
        };
    },
    methods: {
        toggle() {
            this.isActive = !this.isActive;
            this.disabled = !this.disabled;
        }
    },
    components: { 
        NewDiv, 
        SecondDiv
    }
}
</script>

<style>
    .colors {
        display: flex;
        flex-direction: row;
        justify-content: space-around;
    }

    .underline {
        text-decoration: underline;
    }
</style>