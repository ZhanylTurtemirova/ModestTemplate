<template>
  <div>
    <the-header />
    <nuxt/>
    <the-footer/>
  </div>
</template>
<script>
import TheHeader from '@/components/Navigation/TheHeader'
import TheFooter from '@/components/Navigation/TheFooter'
export default {
  components: {
    TheHeader,
    TheFooter
  }
}
</script>

<style>
html { 
  font-family: 'Quattrocento Sans', sans-serif;
  font-size: 10px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}

</style>
