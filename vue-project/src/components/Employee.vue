<script>
export default {
    emits: ['show'],
    data() {
        return {
        }
    },
    methods: {
    }
}
</script>

<template>
<button class="button" @click="$emit('show', 'Jujuba')">name</button>
</template>