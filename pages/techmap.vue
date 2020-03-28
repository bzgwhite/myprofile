<template>
    <div>
        <Header />
        <main>
            <logo />
            <h1>Techmap</h1>
            <section>
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
import Header from '@/components/header.vue'
import Footer from '@/components/footer.vue'

export default ({
    components: {
        Logo,
        Header,
        Footer
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

section{
    margin: 2em auto;
}

h2{
    text-align: center;
    color: white;
}
</style>