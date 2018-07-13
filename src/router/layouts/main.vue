<script>
import NavBar from '@components/nav-bar'
import NavBarAdditional from '@components/nav-bar-additional'

export default {
  components: {
    NavBar,
    NavBarAdditional,
  },
}
</script>

<template>
  <div :class="$style.container">
    <NavBar/>
    <NavBarAdditional/>
    <slot/>
  </div>
</template>

<style lang="scss" module>
@import '@design';

.container {
  min-width: $size-content-width-min;
  max-width: $size-content-width-max;
  margin: 10px auto;
  text-align: center;
}
</style>
