<template>
  <div id="todo-app">
    <h1>ToDosss</h1>
    <section>
      <ul>
        <li><ToDoItem label="Hello" v-bind:done="false" /></li>
        <li><ToDoItem label="Lagi" v-bind:done="true" /></li>
        <li><ToDoItem label="Bambang" v-bind:done="false" /></li>
      </ul>
    </section>
  </div>
</template>

<script>
import ToDoItem from './components/ToDoItem.vue'
export default {
  name: 'ToDoApp',
  components: {
    ToDoItem
  }
}
</script>
