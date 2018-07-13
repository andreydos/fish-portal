<script>
import NavBarRoutes from './nav-bar-routes.vue'

export default {
  components: { NavBarRoutes },
  data() {
    return {
      persistentNavRoutes: [
        {
          name: 'test1',
          title: 'Test #1',
        },
        {
          name: 'test2',
          title: 'Test #2',
        },
      ],
    }
  },
}
</script>

<template>
  <ul :class="$style.container">
    <NavBarRoutes :routes="persistentNavRoutes"/>
  </ul>
</template>

<style lang="scss" module>
@import '@design';

.container {
  padding: 0;
  margin: 0 0 $size-grid-padding;
  text-align: center;
  list-style-type: none;

  > li {
    display: inline-block;
    margin-right: $size-grid-padding;
  }
}
</style>
