<template lang="pug">
  .container
    .wrapper.flex
      UserMenu(:imageUrl="imageUrl")
      .menu
        UserInfo
        UserStats
        CreatePost(:yourUrl="yourUrl")
        UserPosts
    .admin-panel
      .user-image.flex.justify-between.mb-3
        h1 User image Url:
        input(v-model="imageUrl")
      .your-image.flex.justify-between
        h1 Your image Url:
        input(v-model="yourUrl")
    
</template>

<script>
import UserMenu from '~/components/UserMenu'
import UserInfo from '~/components/UserInfo'
import UserStats from '~/components/UserStats'
import CreatePost from '~/components/CreatePost'
import UserPosts from '~/components/UserPosts'

export default {
  components: {
    UserMenu,
    UserInfo,
    UserStats,
    CreatePost,
    UserPosts,
  },
  data() {
    return {
      imageUrl:
        'https://sun1-27.userapi.com/s/v1/if1/5GT7J0b_wlUBY7gD-HULqgkSjq5AKWozDPrhzVeltytyw6sfQywpY-6PUysBOGyq-JGLS0l5.jpg?size=200x0&quality=96&crop=0,0,960,1280&ava=1',
      yourUrl:
        'https://sun1-83.userapi.com/s/v1/if1/kIlCdSOPsuHtjml2ga4qEJiEqOTo999pGteV-MAJMPpb2Mk9yI72jLLgXFGs-y-liXuo8v7X.jpg?size=50x0&quality=96&crop=3,116,742,742&ava=1',
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
