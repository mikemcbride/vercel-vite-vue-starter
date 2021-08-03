<template>
    <div class="w-full max-w-3xl mx-auto">
        <img alt="Vue logo" class="mx-auto my-12" src="./assets/logo.png" />
        <HelloWorld msg="Vue + Vite + Tailwind Starter" />
    </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
    name: 'App',
    components: {
        HelloWorld,
    },
    mounted() {
        const { timeZone, locale } = Intl.DateTimeFormat().resolvedOptions()
        fetch('/api/pageview', {
            method: 'POST',
            body: JSON.stringify({ timeZone, locale }),
            headers: { 'Content-Type': 'application/json' },
        })
    },
}
</script>
