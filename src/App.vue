<template>
  <div id="app" class="full-height clearfix">
    <div class="navMenu fl full-height">
        <NavMenu></NavMenu>
    </div>
    <div class="content full-height">
        <router-view/>
    </div>
  </div>
</template>

<script>
    import NavMenu from './view/NavMenu'

    export default {
        name: 'App',
        components:{
            NavMenu
        }
    }
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>

<style scoped lang="less">
    @navWidth: 200px;
    .navMenu{
        width: @navWidth;
        float: left;
        background: #545c64;
    }
    .content{
        margin-left: @navWidth;
    }
</style>
