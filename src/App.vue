<script setup lang="ts">
  // type MyPick<T, K extends keyof T> = {
  //   [P in K]: T[P]
  // }

  interface Todo {
    title: string
    description: string
    completed: boolean
  }

  type A = Pick<Todo, 'title' | 'completed'>

  const a: A = {
    title: 'dsdad',
    completed: false
  }
</script>

<template>
  <div>
    {{ a }}
  </div>
</template>

<style scoped></style>
