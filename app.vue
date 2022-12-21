<script setup>
  import { nanoid } from 'nanoid'
  const id = nanoid()
  console.log(id)
</script>

<template>
  <input style="width:100%" type="text" v-bind-once="{ id, name: id, value: id }" />
  <label v-bind-once="{ for: id }" />
</template>
