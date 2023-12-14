<script setup>

import router from '@/router';
import { useRouter } from 'vue-router'

defineProps(["event"])

const register = () => {
    // If registration API call is successful
    // Push back to the event details
    router.replace({
        name: 'EventDetails',
    })
}

</script>

<template>
    <p>Register the event</p>
    <button @click="register">Register Me!</button>
</template>