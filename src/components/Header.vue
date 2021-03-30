<template>
  <header>
    <h1>{{title}}</h1>
    <Button text="Add task" color="green" />
  </header>
</template>

<script>
import Button from './Button'

export default {
    name: 'Header',
    props: {
        title: String /* title: {type: String, default: 'Hello World'} */
    },
    components: {
        Button
    }
}
</script>

<style scoped>
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
}
</style>
