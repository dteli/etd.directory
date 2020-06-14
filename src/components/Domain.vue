<template>
  <li>
    <h2>{{ domain.name }}</h2>
    <h3>{{ domain.registrar }}</h3>
    <p>currently {{ domain.inUse ? "in use" : "on ice" }}
    <p>{{ domain.description }}</p>
  </li>
</template>

<script lang="ts">
import { Component, Vue, Prop } from 'vue-property-decorator'
import { DomainData } from '@/types'

@Component
export default class Domain extends Vue {
  @Prop(DomainData) readonly domain: DomainData
}
</script>

<style scoped lang="scss">

li {
  display: block;
  border: .4rem solid black;
  border-radius: 10px;
}

</style>
