<template>
    <list info="Все задачи"></list>
</template>

<script>
    import List from "@/components/List.vue";

    export default {
        name: "AllTask",
        components: { //регистрируем элемет после импорта
            List
        }
    }
</script>

<style scoped>

</style>