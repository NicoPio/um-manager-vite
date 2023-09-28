<template>
  <div>POUET POUET</div>
  <router-view />
</template>

<script lang="ts">
import { Component, Vue, toNative } from 'vue-facing-decorator';

@Component
class App extends Vue {
  name: 'App';

  mounted() {
    console.log('App : mounted')
  }

};
export default toNative(App)

</script>
