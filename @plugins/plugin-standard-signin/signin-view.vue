<template>
  <div class="auth-form">
    <el-signin />
  </div>
</template>
<script lang="ts">
export default {
  components: {
    elSignin: () => import("./signin.vue"),
  },
  metaInfo() {
    return {
      title: "Login / Sign Up",
      description: "Login or register an account.",
    }
  },
}
</script>

<style lang="less">
.auth-form {
  max-width: 400px;
  margin: 2em auto;
  min-height: 75vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
}
</style>
