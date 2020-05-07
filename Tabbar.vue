<template>
    <div class="tab-bar">
    <slot>
    </slot>
  </div>
</template>
<script>
export default {
  name: '',
  data () {
    return {};
  },
  computed: {},
  created () { },
  mounted () { },
  methods: {}
};
</script>
<style scoped>
.tab-bar {
  height: 49px;
  position: fixed;
  left: 0;
  right: 0;
  bottom: 0;
  font-size: 12px;
  display: flex;
  background-color: #edebed;
  box-shadow: 0 -1px 2px rgba(100, 100, 100, 0.2);
  text-align: center;
}
</style>
