<template>
  <Person name="Sajib" age="26">
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Velit ipsa quia, iste veniam earum id vel esse pariatur assumenda, quas minima magnam! Nobis quia maxime pariatur ad corrupti porro modi vel incidunt rem iusto ullam tempora ratione nemo laboriosam quis, soluta eveniet fuga iste laborum? Maiores dolor vel doloremque voluptatibus.</p>
  </Person>
</template>

<script>
import Person from "./components/Person.vue";
export default {
  name: "App",
  components: {
   Person, 
  },
  data() {
    return {

    };
  },
};
</script>
