<template>
    <div>
        <h1 class="remaining">
        {{'You have:  remaining!'}}
      </h1>
      <div class="table">
        <div class="stack">
          {{'renderPlates([])'}}
        </div>
      </div>
    </div>
</template>

<script>

// const renderPlates = (array) => {
//     return array.map((x, index) => {
//       return <div class="empty-plate" style={{ top: -7 * index }}/>
//     })
// }

// if(this.testing){
//     renderPlates()
// }

export default {
    name:'Table',
    data() {
        return {
        }
    }
}
</script>