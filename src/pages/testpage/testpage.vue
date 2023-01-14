<template>
  <view class="testpage">
    <button @click="testOn">button</button>
  </view>
</template>

<script>
import { reactive, toRefs } from 'vue';
import bt from '../../../services/test';


export default {
  name: 'Index',
  components: {
    
  },
  setup() {
    
    const testOn = ()=>{
      bt.close();
    }

    return {
      ...toRefs(state),
      handleClick,
      testOn
    }
  }
}
</script>

<style lang="scss">

</style>
