<template>
  <div>
    <!-- 是否登录 -->
    <login-welome></login-welome>
    <!-- 今日赠言 -->
    <tip></tip>
    <!-- 资源推荐 -->
    <Cat></Cat>
  </div>
</template>

<script>
import Cat from '@/views/cat/Cat'

import LoginWelome from '@/views/card/LoginWelome'
import Promotion from '@/views/card/Promotion'
import Tip from '@/views/card/Tip'

export default {
  name: "CardBar",
  components: {LoginWelome,Promotion,Tip,Cat},
  data() {
    return {
    }
  },
  created() {
  },

  methods: {

  },
};
</script>

<style>

</style>