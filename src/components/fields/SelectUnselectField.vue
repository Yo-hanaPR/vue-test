<template>
  <button @click="notifyParent">Haz clic para habilitar o deshabilitar los campos</button>
</template>
  
  <script setup>
const emit = defineEmits(); 

const notifyParent = () => {
  emit('enable', true);
};
  </script>
  
  <style scoped>
  input {
    margin-right: 10px;
  }
  </style>
  