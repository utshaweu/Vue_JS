<template>
  <Layout>
    <h1>Main Content</h1>
      <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Nesciunt minus modi pariatur dolore tempora facere sint, corporis hic porro et ipsam magni iste. Minus perspiciatis ipsam debitis dolore voluptatum dolor est neque, quibusdam temporibus quas rerum nostrum at consequuntur quasi illo distinctio earum deserunt ullam itaque? Placeat numquam magnam quod.</p>
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

    };
  },
};
</script>
