<template>
    <Header :title="'NAME'"/>
</template>
  
  <script>
  import Header from '@/components/header/Header.vue';
  export default {
    name: 'AppLayout',

    components: {
        Header,
    }
  };
  </script>
  
  