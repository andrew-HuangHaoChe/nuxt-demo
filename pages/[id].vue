<template>
    <div>
        <h1>動態網址</h1>
        {{ route.path }}
    </div>
</template>
<script setup>
    const route = useRoute();
</script>