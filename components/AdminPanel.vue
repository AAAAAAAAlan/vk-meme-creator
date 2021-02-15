<template lang="pug">
  input(v-model="imageUrl")
</template>

<script>
export default {
  data() {
    return {
      imageUrl:
        'https://sun1-27.userapi.com/s/v1/if1/5GT7J0b_wlUBY7gD-HULqgkSjq5AKWozDPrhzVeltytyw6sfQywpY-6PUysBOGyq-JGLS0l5.jpg?size=200x0&quality=96&crop=0,0,960,1280&ava=1',
    }
  },
}
</script>

<style lang="stylus" scoped>
input
  margin-top 30px
  width 100%
</style>
