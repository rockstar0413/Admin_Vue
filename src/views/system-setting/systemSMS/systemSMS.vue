<template>
  <div style="border: 1px solid #eee; padding: 0.75rem; text-align: center;">

    <el-form :model="formData" label-width="100px" style="width: 600px; display: inline-block;">
      <el-form-item label="手机号码">
        <el-input v-model="formData.accountNumber" placeholder="" clearable></el-input>
      </el-form-item>

      <el-form-item label="内容">
        <el-input type="textarea" autosize placeholder="Please input message" v-model="formData.message"></el-input>
      </el-form-item>
      <el-form-item style="display: inline-flex;">
        <el-button type="primary">立即发送</el-button>
        <el-button type="danger">重置</el-button>
      </el-form-item>
    </el-form>
  </div>
</template>

<script>
export default {
  data() {
    return {
      formData: {
        accountNumber: '',
        title: '',
        message: '',
      },
    }
  },
}
</script>

<style lang="scss" scoped></style>
