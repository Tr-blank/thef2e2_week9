<template lang="pug">
  .app
    header
      h1 MARKDOWN
      a.header__botton 建立筆記
      nav.nav
        a.nav__item 所有筆記
        a.nav__item 已加星號
        a.nav__item 垃圾桶
    main.folder
      .folder__header
        .folder__list
          .folder_item 123
</template>

<script>

import './assets/style/normalize.css'
import './assets/style/reset.css'

export default {
  name: 'App',
  components: {
  },
  data () {
    return {
    }
  },
  created () {

  },
  mounted () {
  },
  computed: {

  },
  methods: {
  }
}
</script>

<style lang="stylus">
body
  background: #25272C;
  color: #F3F2EF;
  font: Regular 16px/24px Noto Sans TC Regular;
  letter-spacing: 1.6px;
  font-size: 16px;

</style>

<style lang="stylus" scoped>
.app
  display: flex;
  height: 100vh;
header
  width: 20%;
  padding: 40px 45px 0
  text-align: center;
  background: #2F3136;
.folder
  width: 80%;
  padding: 52px 30px;
h1
  color: #84A5FF;
.header__botton
  display: block;
  background: #84A5FF;
  border-radius: 30px;
  color: #fff;
  line-height: 52px;
  margin: 40px 0;
.nav__item
  display: block;
  margin-bottom: 12px;
.breadcrumbs
  &__item
    color: #F3F2EF;
    opacity: .5;
    &::after
      content: '';
      border-color: transparent #f3f2ef;
      margin: 0 10px;
      border-style: solid;
      border-width: 4px 0px 4px 6px;
      display: inline-block;
    &--now
      opacity: 1;
      &::after
        display: none;

</style>
