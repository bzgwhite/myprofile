<template>
    <div>
        <Header />
        <main class="change_font">
            <logo />
            <h1>Techmap</h1>
            <section class="techmap_area">
                <h2>language</h2>
                <ul>
                    <li>HTML(2016~)</li>
                    <li>CSS(2016~)</li>
                    <li>Ruby(2016~)</li>
                    <li>Google Apps Script(2017~)</li>
                    <li>JavaScript(2017~)</li>
                    <li>PHP(2017~)</li>
                    <li>Objective-C(2017~)</li>
                    <li>node.js(2019~)</li>
                    <li>Python(2019~)</li>
                    <li>TypeScript(2020~)</li>
                </ul>
                <h2>FrameWork</h2>
                <ul>
                    <li>Ruby On Rails(2016~)</li>
                    <li>wordpress(2018~)</li>
                    <li>vue.js(2019~)</li>
                    <li>nuxt.js(2020~)</li>
                </ul>
                <h2>others</h2>
                <ul>
                    <li>git(2017~)</li>
                    <li>linux(2019~)</li>
                    <li>Vagrant(2019~)</li>
                    <li>docker(2019~)</li>
                    <li>Selenium(2019~)</li>
                    <li>Google compute engine(2019~)</li>
                </ul>
            </section>
        </main>
        <Footer />
    </div>
</template>

<script lang="ts">
import Logo from '~/components/Logo.vue'

export default ({
    components: {
        Logo
    }
})
</script>

<style>
main{
    padding-top: 34px;
}
main img{
    display: flex;
    flex-direction: column;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
    width: 100%;
    height: 100%;
}

h1,h2{
    margin-bottom: 1em;
}

h2{
    text-align: center;
    color: white;
}

.techmap_area{
    display: flex;
    align-items: center;
    flex-direction: column;
    margin: 2em auto;
}
.techmap_area ul{
    text-align: left;
    padding: 0;
    width: 50%;
    margin-bottom: 1em;
}
.techmap_area li{
    list-style: none;
}

</style>