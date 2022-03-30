<template>
    <header>
        <img  class='logo' src="https://upload.wikimedia.org/wikipedia/commons/thumb/8/84/Spotify_icon.svg/512px-Spotify_icon.svg.png?20191006032433" alt="">
    </header>
</template>

<script>
export default {
    name : 'HeaderIndex',
}
</script>

<style scoped lang="scss">
header{
    height: 8vh;
    background-color: #2e3a46;
    text-align: left;
    .logo{
        height: 100%;
        padding: 1rem;
        margin-left: 0.5rem;
    }
}
</style>