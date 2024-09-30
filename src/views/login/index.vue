<template>
  <div class="flex justify-center items-center h-full">
    <el-form :model="userInfo" label-width="100px">
      <el-form-item label="用户名：" prop="pass">
        <el-input v-model="userInfo.username" placeholder="用户名" />
      </el-form-item>
      <el-form-item label="密码：" prop="password">
        <el-input v-model="userInfo.password" placeholder="密码" />
      </el-form-item>
      <el-form-item>
        <el-button type="primary" @click="handleLogin">登录</el-button>
        <el-button @click="handleUp">注册</el-button>
      </el-form-item>
    </el-form>
  </div>
</template>

<script>
export default {
  name: 'Login',
  data() {
    return {
      userInfo: {
        username: '',
        password: '',
      },
    };
  },
  methods: {
    handleLogin() { },
    handleUp() { },
  },
};
</script>

<style></style>
