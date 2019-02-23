<template>
    <div class="sign-in-component">
        <el-form status-icon label-width="100px" class="demo-ruleForm">
            <el-form-item label="用户名">
                <el-input type="text" v-model="username" autocomplete="on"></el-input>
            </el-form-item>
            <el-form-item label="用户名">
                <el-input type="password" v-model="password" autocomplete="on"></el-input>
            </el-form-item>
            <el-form-item>
                <el-button type="primary" @click="submitForm">提交</el-button>
            </el-form-item>
        </el-form>
    </div>
</template>

<script>
  export default {
    data() {
      return {
        username:'',
        password:''
      };
    },
    methods: {
      submitForm(){}
    }
  }
</script>