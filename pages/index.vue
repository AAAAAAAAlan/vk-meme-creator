<template lang="pug">
  .container
    .wrapper.flex
      UserMenu(:imageUrl="imageUrl")
      .menu
        UserInfo
        UserStats
    .admin-panel.flex.justify-between
      h1 Image Url:
      input(v-model="imageUrl")
</template>

<script>
import UserMenu from '~/components/UserMenu'
import UserInfo from '~/components/UserInfo'
import UserStats from '~/components/UserStats'

export default {
  components: {
    UserMenu,
    UserInfo,
    UserStats,
  },
  data() {
    return {
      imageUrl:
        'https://sun1-27.userapi.com/s/v1/if1/5GT7J0b_wlUBY7gD-HULqgkSjq5AKWozDPrhzVeltytyw6sfQywpY-6PUysBOGyq-JGLS0l5.jpg?size=200x0&quality=96&crop=0,0,960,1280&ava=1',
    }
  },
}
</script>

<style lang="stylus" scoped>
.admin-panel
  margin-top 50px
  input
    width 90%
  h1
    width 10%
</style>
