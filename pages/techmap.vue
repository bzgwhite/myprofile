<template>
    <div>
        <Header />
        <main>
            <logo />
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
main img{
    display: flex;
    flex-direction: column;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
    width: 100%;
    height: 100%;
}
</style>