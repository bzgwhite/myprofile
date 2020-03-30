<template>
    <div>
        <Header />
        <main>
            <logo />
            <h1>What's Black Dragon?</h1>
            <section>
                <p>BlackDragon born in Japan.</p>
                <p>Japanese Software Engineer.</p>
                <p>I belong to a software development company.</p>
                <p>I'd like to become famous developer.</p>
                <p>I'd like to release a usable app.</p>
                <p>I'd like to change our life very fun.</p>
            </section>
            <section>
                <p>I love karaoke.</p>
                <p>And drink a alcohol.</p>
                <p>My President is Mr.Soyokaze.</p>
                <p>Alcohol make me happy!</p>
                <p>Computer make me happy!</p>
                <p>Karaoke make me happy!</p>
                <p>Reading book make me happy!</p>
                <p>Sleeping make me happy!</p>
                <p>Running make me happy!</p>
                <p>Walking make me happy!</p>
                <p>BasketBall make me happy!</p>
                <p>Hospital make me happy!</p>
                <p>Party make me happy!</p>
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
h1,p{
    color:#fff;
    text-align: center;
}
</style>