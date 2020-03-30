<template>
    <div>
        <Header />
        <main>
            <logo />
            <h1>My History</h1>
            <div class="history_area">
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
            </div>
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
h1,li{
    color:#fff;
}

h1,h2{
    margin-bottom: 1em;
}

.history_area{
    display: flex;
    align-items: center;
    flex-direction: column;
}
.history_area ul{
    text-align: left;
    padding: 0;
    width: 50%;
    margin-bottom: 1em;
}
.history_area li{
    list-style: none;
}

</style>