<template>
    <div>
<!--only one elemnt-container unchanged part-->
        <div>
            <p>Всего задач: {{tasks.length}}</p>
            <nav>
                <router-link to="/add/task">Создать задачу</router-link>
                <router-link to="/show/task">Просмотр задач</router-link>
            </nav>
        </div>


    <!--подгружаемый контент-->
    <div>
        <router-view></router-view>
    </div>
    </div>

</template>

<script>
    import {allTasks} from "./tmp/taskArr";

    export default {
        name: "App", //имя файла без расширения
        data: function () {
            return {
                tasks: allTasks
            }
        }
    }
</script>

<style lang="scss">

</style>
