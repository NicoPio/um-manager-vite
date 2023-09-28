<template>
  <div>POUET POUET</div>
  <router-view />
</template>

<script lang="ts">
// import { defineComponent } from 'vue';
import { Component, Vue } from 'vue-facing-decorator';

@Component
export default class App extends Vue {
  name: 'App';

  mounted() {
    console.log('App : mounted')
  }

};

</script>
