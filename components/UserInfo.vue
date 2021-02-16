<template lang="pug">
  .user-menu
    .upper-container.flex.justify-between.items-center
      h1.name(contenteditable spellcheck="false") Ильяс Юзбашев
      p.last-onlone(contenteditable spellcheck="false") заходил сегодня в 2:58
    p.status(contenteditable spellcheck="false") настоящее имя равиль
    .line
    .info-block.flex.justify-start
      .info-title
        p День рождения:
        p Город:
        p Место работы:
      .info
        p 21 октября 1993г.
        p(contenteditable spellcheck="false") Кишинёв
        p(contenteditable spellcheck="false") Empire of Stasyan (Стас / Stas)
        p.more Показать подробную информацию
</template>

<style lang="stylus" scoped>
.user-menu
  margin-right 15px !important
  padding 15px 20px
  width 550px
  height 210px
  background #fff
  border-radius 4px 4px 0 0
  box-shadow 0 1px 0 0 #d3d9de,0 0 0 1px #e7e8ec
  margin 15px 0 1px 0
  .name
    font-size 19px
    font-weight 400
  .status
    margin-top 5px
    font-size 13px
  .info-block
    font-size 13px
    p
      margin-top 10px
    .info-title
      margin-right 70px
      color #828282
    .info
      color #2a5885
      .more
        margin-top 20px
  .line
    width 100%
    height 1px
    background-color #e7e8ec
    margin 20px 0
  .upper-container
    p
      margin-top 2px
      font-size 12.5px
      color #939393
</style>
