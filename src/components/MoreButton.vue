<template>
    <button @click="$emit('next-sushi')">
            More sushi!
    </button>
</template>

<script>
export default {
    name:"MoreButton"
}
</script>