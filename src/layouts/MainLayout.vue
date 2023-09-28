<template>
  <q-layout view="lHh Lpr lFf">
    <q-header elevated>
      HEADER
    </q-header>

    <q-drawer v-model="leftDrawerOpen" show-if-above bordered>
      Drawer
    </q-drawer>

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script lang="ts">
import { Component, Vue, toNative } from 'vue-facing-decorator'

@Component({
  name: 'MainLayout'
})
class MainLayout extends Vue {
  leftDrawerOpen = false
  toggleLeftDrawer() {
    this.leftDrawerOpen = !this.leftDrawerOpen
  }

}

export default toNative(MainLayout)
</script>
