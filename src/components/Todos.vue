<template lang="html">
    <div class="container">
        <div v-bind:key="todo.id" v-for="todo in todos">
            <TodoItem />
        </div>
    </div>
</template>

<script>
import TodoItem from './TodoItem.vue';

export default {
    name: 'Todos',
    components: {
        TodoItem
    },
    props: ['todos']
}
</script>

<style lang="css" scoped>
</style>
