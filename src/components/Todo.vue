<script>
export default {
    props: {
        todos: Array,
    },
};
</script>

<template>
    <ul>
        <li v-for="todo in todos" :key="todo.id">
            {{ todo.text }}
            <input type="checkbox" :checked="todo.isDone" />
        </li>
    </ul>
</template>

<style lang="scss" scoped></style>
