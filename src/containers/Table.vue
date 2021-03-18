<template>
    <div>
        <h1 class="remaining">
        {{`You have: $${money}`}}
      </h1>
      <div class="table">
        <div class="stack">
          <div 
            class="empty-plate" 
            :style="{'top': -7 * eatenSushi.indexOf(sushi) + 'px'}" 
            v-bind:key="sushi.id" 
            v-for="sushi in eatenSushi"/>
        </div>
      </div>
    </div>
</template>

<script>

export default {
    name:'Table',
    props:["eatenSushi", "money"],
    methods:{
      // countPlate(sushi) {
      //   return {
      //     top: -7 * this.eatenSushi.indexOf(sushi)
      //   }
      // }
    }
}
</script>