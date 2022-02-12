<template>
  <div class="border relative border-dashed border-indigo-500 p-10 mt-4">
    <a @click="$emit('close', 10)" href="#" class="text-2xl font-bold text-red-500 absolute top-0 right-2">&times;</a>
    <h1 class="text-4xl font-semibold">My name is {{name}}</h1>
    <h1 class="text-2xl font-semibold">Age: {{age}}</h1>
    <slot/>
  </div>
</template>


<script>
export default {
  props: ['name', 'age'],
}
</script>