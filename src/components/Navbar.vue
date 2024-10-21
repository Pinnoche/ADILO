<script setup lang="ts">
import { useRoute } from 'vue-router';
const route = useRoute();

    
</script>

<template>
    <div class="nav">
        <h1>{{route.name}}</h1>
        <div>
            <img src="@/assets/images/download.png" alt="Download">
            Download
        </div>
    </div>
</template>

<style scoped>
.nav {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding-bottom: 2rem;
    border-bottom: 1px #0000001A solid;
}

.nav div {
    display: flex;
    align-items: center;
    gap: 2px;
    cursor: pointer;
}

.nav img {
    cursor: pointer;
}

</style>