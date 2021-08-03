<template>
    <h1 class="text-4xl font-bold mb-8 text-center">{{ msg }}</h1>

    <h2 class="text-2xl font-bold mb-8">Docs</h2>
    <ul class="my-8 list-disc space-y-2 ml-6 text-xl">
        <li>
            <a
                href="https://vitejs.dev/guide/features.html"
                class="text-blue-600 hover:underline hover:text-blue-700"
                target="_blank"
                >Vite</a
            >
        </li>
        <li>
            <a
                href="https://v3.vuejs.org/"
                class="text-blue-600 hover:underline hover:text-blue-700"
                target="_blank"
                >Vue 3</a
            >
        </li>
        <li>
            <a
                href="https://tailwindcss.com/docs/"
                class="text-blue-600 hover:underline hover:text-blue-700"
                target="_blank"
                >Tailwind</a
            >
        </li>
        <li>
            <a
                href="https://headlessui.dev/"
                class="text-blue-600 hover:underline hover:text-blue-700"
                target="_blank"
                >Headless UI</a
            >
        </li>
        <li>
            <a
                href="https://heroicons.com/"
                class="text-blue-600 hover:underline hover:text-blue-700"
                target="_blank"
                >Heroicons</a
            >
        </li>
    </ul>

    <h2 class="text-2xl mb-4 font-bold">Getting Started</h2>
    <p class="mb-8 leading-normal text-xl">
        Before you get started, there are a couple of housekeeping things to
        update on this template:
    </p>
    <ul class="my-8 list-disc space-y-2 ml-6 text-xl">
        <li>Update the title tag in index.html</li>
        <li>Delete this component and remove it from App.vue</li>
        <li>Delete logo.png in the /src/assets folder</li>
    </ul>

    <p class="my-8 leading-normal text-xl">
        Now you're ready to build your app! Tailwind is already configured and
        ready to go, and we've even got the Tailwind Forms plugin installed too.
        Headless UI and Heroicons Vue libraries are already installed so you can
        import those in your components and get straight to work. The API
        directory is set up and a pageview function is there as an example for
        logging pageview to analytics. App.vue makes a call to that endpoint on
        the mounted hook, and this is ready to be deployed directly to Vercel.
    </p>
</template>

<script setup>
import { defineProps } from 'vue'

defineProps({
    msg: String,
})
</script>
