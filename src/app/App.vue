<script setup lang="ts">
    import { computed } from 'vue';
    import { RouterView, useRoute } from 'vue-router';
    import { DefaultLayout } from '@/shared';

    const route = useRoute();

    const layout = computed(() => {
        return route.meta.layout || DefaultLayout;
    });
</script>

<template>
    <component :is="layout">
        <RouterView />
    </component>
</template>
