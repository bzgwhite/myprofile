<template>
    <header>
        <ul>
            <li v-for="item in items" v-bind:key="item.title">
                <nuxt-link v-bind:to="item.link">{{ item.title }}</nuxt-link>
            </li>
        </ul>
    </header>
</template>


<script lang="ts">

export default ({
    data:function(){
        return {
            items:[
                {
                    title:"Home",
                    link:"/"
                },
                {
                    title:"About",
                    link:"about"
                },
                {
                    title:"History",
                    link:"history"
                },
                {
                    title:"Techmap",
                    link:"techmap"
                }
            ]
        }
    }
})
</script>

<style>
header{
    position: fixed;
    width: 100%;
}

header ul {
    display:flex;
    justify-content: space-around;
    padding: 0;
}

header li{
    list-style: none;
    margin: 0.5em 0;
}

header li a{
    text-decoration: none;
    color: azure;
}
</style>