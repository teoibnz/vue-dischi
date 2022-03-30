<template>
    <main>
        <Cover/>
    </main>
</template>

<script>
import Cover from './Cover.vue'

export default {
    name : 'CoverList',
    components : {
        Cover,
    } 
}
</script>

<style scoped lang='scss'>
main{
    background-color: #1e2d3b;
    height: 92vh;
}
</style>