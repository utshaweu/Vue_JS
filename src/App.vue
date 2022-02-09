<template>
  <div class="p-10">
    <h1 class="text-3xl font-bold">Hello vue js</h1>
    <h1 class="font-medium">Count: {{ count }}</h1>
    <button
      @click="count++"
      class="bg-violet-500 hover:bg-violet-400 active:bg-violet-600 focus:outline-none focus:ring focus:ring-violet-300 px-5 py-2 mt-2 mr-2 rounded-3xl text-white font-bold"
    >
      Addition
    </button>
    <button
      @click="count--"
      class="bg-sky-600 hover:hover:bg-sky-700  active:hover:bg-sky-600  focus:outline-none focus:ring focus:hover:bg-sky-300 px-5 py-2 mt-2 rounded-3xl text-white font-bold"
    >
      Deduction
    </button>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      count: 0,
    };
  },
};
</script>
