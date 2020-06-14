<template>
  <div class="main-div">
    <h1>Domains</h1>
    <p>general blurb goes here</p>
    <ul>
      <Domain v-for="(d, i) of domains"
        :key="i"
        :domain="d" />
    </ul>
  </div>
</template>

<script lang="ts">
import { Component, Vue, Prop } from 'vue-property-decorator'
import Domain from '@/components/Domain.vue'
import { DomainData } from '@/types'

@Component({
  name: 'Domains',
  components: {
    Domain
  }
  // props: {
  //   domains: {
  //     type: Array<DomainData>
  //   }
  // }
})
export default class Domains extends Vue {
  @Prop(Array) readonly domains: Array<DomainData>
}
</script>
