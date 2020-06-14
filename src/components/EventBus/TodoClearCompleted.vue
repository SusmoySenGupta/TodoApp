<template>
  <div>
    <button class="btn" v-if="showClearCompletedButton" @click="clearCompleted()">Clear Completed</button>
  </div>
</template>
<script>
export default {
  name: "todo-clear-completed",
  props: {
    showClearCompletedButton: {
      type: Boolean,
      required: true
    }
  },
  methods: {
    clearCompleted() {
      eventBus.$emit("clearCompletedTodos");
    }
  }
};
</script>