<template>
    <div class="todo-item" v-bind:class="{'is-complete':aTask.completed}">
        <p>
            <input type="checkbox" v-on:click="markComplete">
            {{aTask.title}}
        </p>
    </div>
</template>

<script>
export default {
    name:"task",
    props:['aTask'],
    methods:
    {
        markComplete(){
            this.aTask.completed = !this.aTask.completed;
        }
    }
}
</script>

<style scoped>
    .todo-item{
        background: #f4f4f4;
        padding: 10px;
        border-bottom: 1px #ccc dotted;
    }

    .is-complete{
        text-decoration: line-through;
    }
</style>