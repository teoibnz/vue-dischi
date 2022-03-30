<template>
    <main>
        <div class="container">
            <div class="card-wrapper" v-for='(element, index) in coverList' :key="index">
                <Cover/>
            </div>
        </div>
        
    </main>
</template>

<script>
import Cover from './Cover.vue'
import axios from 'axios';


export default {
    name : 'CoverList',
    components : {
        Cover,
    },
    data: function(){
        return {
            coverList : null
        }
    },
    created: function(){
    this.getCoverApi();
    },
    methods: {
    getCoverApi(){
        axios.get('https://flynn.boolean.careers/exercises/api/array/music')
        .then((result) => {
        console.log(result.data.response)
        this.coverList = result.data.response;
        })
    }
    }
    
}
</script>

<style scoped lang='scss'>
main{
    background-color: #1e2d3b;
    height: 92vh;
    .container{
        width: 65%;
        margin: 0 auto;
        display: flex;
        flex-wrap: wrap;
        .card-wrapper{
        width: calc(100% / 5);
        
    }
    }
    
}
</style>