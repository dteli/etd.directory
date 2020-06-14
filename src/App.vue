<template>
  <div id="app">
    <Sidebar />
    <router-view/>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'

import Sidebar from '@/components/Sidebar.vue'

@Component({
  components: {
    Sidebar
  }
})
export default class App extends Vue {

}
</script>

<style lang="scss">
* {
  box-sizing: border-box;
}

html {
  font-size: 12px;
}

body {
  margin: 0;
}

#app {
  display: flex;
}
</style>
