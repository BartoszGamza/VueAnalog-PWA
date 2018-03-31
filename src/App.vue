<template>
  <div id="app">
    <header class="header">
      <nav class="inner">
        <router-link to="/">HOT</router-link>
        <router-link to="/rising">RISING</router-link>
        <router-link to="/new">NEW</router-link>
        <router-link to="/controversial">CNTR</router-link>
        <router-link to="/top">TOP</router-link>
        <router-link to="/gold">GOLD</router-link>
      </nav>
    </header>
    <router-view class="view"/>
  </div>
</template>

<style lang="stylus">
body
  font-family: 'Roboto', sans-serif
  font-size 15px
  background-color #f8f8fa
  margin 0
  padding-top 25px
  color #afafaf
  overflow-y scroll

.header
  background-color white
  position fixed
  z-index 999
  height 25
  top 0
  left 0
  right 0
  box-shadow 0 1px 3px rgba(0,0,0,0.12), 0 1px 2px rgba(0,0,0,0.24)
  .inner
    max-width 500px
    box-sizing border-box
    margin 0px auto
    text-align center
    padding 15px 5px
  a
    text-decoration none
    color #afafaf
    line-height 24px
    display inline-block
    vertical-align middle
    font-weight 300
    letter-spacing .075em
    padding-left 5px
    padding-right 5px
    &:hover
      color #8c8c8c
.view
  max-width 500px
  margin 0 auto
  position relative
</style>
