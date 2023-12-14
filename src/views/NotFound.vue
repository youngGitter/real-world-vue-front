<script setup>
defineProps({
    resource: {
        type: String,
        required: true,
        default: 'page'
    }
})
</script>

<template>
    <h1>Opps!</h1>
    <h3>The {{ resource }} Not Found Here.</h3>
    <router-link :to="{ name: 'EventList' }">Back to home page</router-link>
</template>
