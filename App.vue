<script>
import Sunshine from './components/Sunshine'
import Moon from './components/Moon'

export default {
  data() {
    return {
      svalue: false
    };
  },
  components: {
    Sunshine,
    Moon
  },
  methods: {
    handleChange() {
      this.svalue = !this.svalue;
    }
  }
};
</script>

<template>
    <view class="container"
          :class="svalue ? 'light-view' : 'dark-view'">
        <switch
            :on-value-change="handleChange"
            :value="svalue"/>
          <sunshine v-if="svalue"/>
          <moon v-else/>
    </view>
</template>
 
<style>
.container {
  align-items: center;
  justify-content: center;
  flex: 1;
}

.light-view {
  background-color: #4EABFF
}
.dark-view {
  background-color: #0B023E
}
</style>
