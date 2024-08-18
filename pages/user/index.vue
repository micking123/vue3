<template>
    <div class="user_index">
        user_index
    </div>
</template>
<script setup lang="ts">
const { data: userData } = useAsyncData('user-data', () => getUserData())
const getUserData = async () => {
    return await $fetch('http://localhost:3000/api/getArticleList1', {
    method: 'get'
    })
}
</script>
<style scoped>

</style>