<template>
    <div>
        <ul>
            <li>
                <nuxt-link exact to="/">Home</nuxt-link>
            </li>
            <li><nuxt-link exact to="/projects">Projects</nuxt-link></li>
        </ul>
    </div>
</template>

<script>
export default {
    
}
</script>

<style scoped>
div {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100vw;
    height: 100px;
    background: #1a7ed6;
}
ul {
    padding-left: 0;
}
li {
display: inline-block;
margin-right: 30px;
}
</style>