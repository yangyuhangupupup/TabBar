<template>

   <div class="tabbar-item"
       @click="itemclick">
    <div v-if="!isActive">
      <slot name="icon-image"></slot>
    </div>
    <div v-else>
      <slot name="active-image"></slot>
    </div>
    <div :style="activeStyle">
      <slot name="icon-text"></slot>
    </div>
  </div>

</template>
<script>
export default {
  name: '',
  data () {
    return {

    };
  },
  props: {
    path: String,
    activeColor: {
      type: String,
      default: 'red'
    }
  },
  computed: {
    isActive () {
      return this.$route.path.indexOf(this.path) !== -1
    },
    activeStyle () {
      return this.isActive ? { color: this.activeColor } : {}
    }
  },
  created () { },
  mounted () { },
  methods: {
    itemclick () {
      //console.log(this.path);
      this.$router.replace(this.path).catch(err => err)

    }
  }
};
</script>
<style scoped>
.tabbar-item {
  flex: 1;
  margin-top: 5px;
}
.tabbar-item img {
  width: 24px;
  height: 24px;
  vertical-align: middle;
}
</style>
