<template>
  <Layout>

    <h1>Main Content</h1>
      <p class="mb-3">Lorem ipsum dolor sit amet consectetur adipisicing elit. Nesciunt minus modi pariatur dolore tempora facere sint, corporis hic porro et ipsam magni iste. Minus perspiciatis ipsam debitis dolore voluptatum dolor est neque, quibusdam temporibus quas rerum nostrum at consequuntur quasi illo distinctio earum deserunt ullam itaque? Placeat numquam magnam quod.</p>
      <a :href="url" class="bg-indigo-500 text-white py-2 px-4">Click Here</a><br/><br/>

      <button @click="toggle" class="text-white bg-blue-600 hover:bg-blue-500 py-2 px-4 mr-3">toggle</button>

      <Person @close="handlerClosePersonComponent" :name="name" :age="age" v-if="visible"/>

      <template #sidebar-left>
        <h1>Sidebar Left</h1>
      </template>

      <template #sidebar-right>
        <h1>Sidebar Right</h1>
      </template>

  </Layout>
</template>

<script>
import Person from "./components/Person.vue";
import Layout from "./components/Layout.vue";
export default {
  name: "App",
  components: {
   Person, 
   Layout,
  },
  data() {
    return {
      url: "https://google.com",
      name: "Sajib",
      age: 26,
      visible: false,
    };
  },
  methods: {
    toggle(){
      this.visible = !this.visible;
    },
    handlerClosePersonComponent(){
      alert("x")
    }
  }
  
};
</script>
