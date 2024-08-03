<template>
  <div
  class="app-wrapper">
  <div
    class="app-wrap_inner">
    <component :is="layout">
      <router-view :key="$route.path" />
    </component>
  </div>
</div>
</template>

<script>
import AppLayout from '@/layouts/AppLayout.vue';
import { AppMixin } from  '@/AppMixin';

export default {
  name: 'App',

  mixins: [AppMixin],

  components: {
    AppLayout,
  },
}
</script>

<style>
</style>
