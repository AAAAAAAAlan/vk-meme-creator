<template lang="pug">
  .user-stats.flex.justify-around
    StatsCard(v-for="(stat, index) in stats" :key="index" :stat="stat")
</template>

<script>
import StatsCard from '~/components/StatsCard'

export default {
  components: {
    StatsCard,
  },
  data() {
    return {
      stats: [
        {
          number: 5,
          text: 'общих друзей',
        },
        {
          number: 69,
          text: 'друзей',
        },
        {
          number: 10,
          text: 'подписчиков',
        },
        {
          number: 32,
          text: 'фотографии',
        },
        {
          number: 21,
          text: 'видеозапись',
        },
      ],
    }
  },
}
</script>

<style lang="stylus" scoped>
.user-stats
  margin-right 15px !important
  padding 15px 20px
  width 550px
  height 70px
  background #fff
  border-radius 0 0 4px 4px
  box-shadow 0 1px 0 0 #d3d9de,0 0 0 1px #e7e8ec
</style>
