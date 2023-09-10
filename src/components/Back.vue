<script>
export default {
    props: {
        wordsJson:Array
    },
    computed: {
        lenList() {
            return ((this.wordsJson.length + 1) * 50 + 100) + "px"
            // return ( 440) + "px"
        }
    },
}
</script>
<template>
    <div class="back" :style="{ height: lenList }"></div>
</template>
<style scoped>
.back {
    position: absolute;
    top: 0;
    left: 0;
    /* background-color: red; */
    width: 1px;
    /* height: 4850px; */
}
</style>