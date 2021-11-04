<template>
    <div class="bg">
        <img :src="picture">
    </div>
</template>

<script>
    export default {
        name: "Banner",
        props: [
            "picture"
        ]
    }
</script>

<style scoped>
</style>