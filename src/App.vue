<template>
  <router-view />
</template>

<script>
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'App'
})
</script>

<style lang="sass">
html, body, #q-app
  width: 100%
  height: 100%
  padding: 0
  margin: 0

::-webkit-scrollbar-track
  background-color: rgba(255, 255, 255, 0)

::-webkit-scrollbar
  width: 6px
  height: 6px
  background-color: #F5F5F5

::-webkit-scrollbar-thumb
  background: rgb(200, 200, 200)
  border-radius: 50px

</style>
