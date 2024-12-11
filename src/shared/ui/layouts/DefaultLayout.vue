<script setup lang="ts">
    import { TheHeader } from '@/widgets/header/';
</script>

<template>
    <div>
        <TheHeader />

        <slot />

        <div>Layout footer</div>
    </div>
</template>
