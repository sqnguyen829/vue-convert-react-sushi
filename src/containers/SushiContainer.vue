<template>
    <div class="belt">
        <div v-bind:key="sushi.id" v-for="sushi in sushis">
            <Sushi 
                v-bind:sushi="sushi" 
                v-bind:eatenSushi="eatenSushi" 
                v-on:eat-sushi="$emit('eat-sushi', sushi)"/>
        </div>
        <MoreButton v-on:next-sushi="$emit('next-sushi')"/>
      </div>
</template>

<script>
import MoreButton from '../components/MoreButton'
import Sushi from '../components/Sushi'

export default {
    name:'SushiContainer',
    components:{
        Sushi,
        MoreButton
    },
    props:["sushis", "eatenSushi"]
}
</script>