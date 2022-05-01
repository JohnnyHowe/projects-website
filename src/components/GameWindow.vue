<template>
    <iframe v-bind:src="link" v-bind:title="title" width="400" height="400"></iframe>
</template>
<script>
export default {
    props: ["link", "title"],
}
</script>
<style scoped>
* {
    border: 0;
}
</style>