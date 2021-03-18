<template>
    <div class="sushi">
      <div class="plate" @click="$emit('eat-sushi', sushi)">
        <div v-if="!eatenSushi.includes(sushi)">
          <img v-bind:src='sushi.img_url' width="100%" />
        </div>
      </div>
      <p class="sushi-details">
        {{sushi.name}}  -  {{sushi.price}}
      </p>
    </div>
</template>

<script>
export default {
  name:"Sushi",
  props:["sushi", "eatenSushi"]
}
</script>