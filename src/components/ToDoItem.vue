<template>
  <article>
    <input type="checkbox" id="todo-item" v-bind:checked="isDone" />
    <label for="todo-item">{{ label }}</label>
  </article>
</template>

<script>
export default {
  name: 'ToDoItem',
  props: {
    label: { required: true, type: String },
    done: { default: false, type: Boolean }
  },
  data() {
    return {
      isDone: this.done
    }
  }
}
</script>
