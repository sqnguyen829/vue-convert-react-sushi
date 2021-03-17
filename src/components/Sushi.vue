<template>
    <div class="sushi">
      <div class="plate" @click="console.log('test')">
        {{ 'check if sushi is eaten'? '' :<img src='something' width="100%" />}}
      </div>
      <h4 class="sushi-details">
        {{'Give me a name!-  Give me a price! '}}
      </h4>
    </div>
</template>