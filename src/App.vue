<template>
  <div id="app">
  <navbar></navbar>
  <list></list>
    <router-view></router-view>
  </div>
</template>

<script>
import Navbar from '@/components/Navbar'
import List from '@/components/List'

export default {
  name: 'app',
  components: {navbar: Navbar, list: List},
}
</script>

<style>
</style>
