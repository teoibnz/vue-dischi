<template>
    <div class="card-items">
        <img :src="cover.poster" alt="">
        <h2>{{cover.title}}</h2>
        <span>{{cover.author}}</span>
        <h5>{{cover.year}}</h5>
    </div>
</template>

<script>
export default {
    name : 'CoverIndex',
    props: {'cover' : Object}
}
</script>

<style scoped lang='scss'>
.card-items{
    height: 350px;
    background-color: #2e3a46;
    margin: 0.5rem;
    img{
        width: 100%;
        height: 250px;
    }
    h2{
        color:white
    }
    span, h5{
        color:#67727d
    }
}

</style>