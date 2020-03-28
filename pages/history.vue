<template>
    <div>
        <Header />
        <main>
            <logo />
            <h1>My History</h1>
            <ul>
                <li>1989.X I've born at Tokyo</li>
                <li>2012.3 I've graduated from University.</li>
                <li>2012.4 I've belong to a System Integrator and Sales Division.</li>
                <li>2018.4 I've change the jobs and become developer</li>
                <li>2019.X I've 30 years old</li>
                <li>2020.3 This Portfolio 0.1 release.</li>
            </ul>
            <h2>Next generation</h2>
            <ul>
                <li>2020.X I will learn machine learning.</li>
                <li>2020.X I will learn DevOps.</li>
                <li>2020.X I will learn MlOps.</li>
                <li>2020.X I will learn Backend more.</li>
                <li>2020.X I will learn Frontend more.</li>
                <li>2020.X I will learn Computer Science more.</li>
                <li>2020.X I will learn DataBase more.</li>
                <li>2020.X I will learn Architecture more.</li>
                <li>2020.X I will learn Healthcare more.</li>
                <li>2020.X I will learn IoT.</li>
                <li>2020.X I will learn Fashion.</li>
                <li>2020.X I will learn about happiness.</li>
            </ul>
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
h1,li{
    color:#fff;
}
ul{
    margin: 0 auto;
}
li{
    list-style: none;
}

</style>