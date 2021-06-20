<template>
  <div style="margin: 20px;">
    <el-input v-model="input" placeholder="请输入内容"></el-input>
    <el-steps :active="2">
      <el-step title="步骤 1" description="这是一段很长很长很长的描述性文字">
        <template slot="iconImg">
          <i class="el-icon-s-platform"></i>
        </template>
      </el-step>
      <el-step title="步骤 2" description="这是一段很长很长很长的描述性文字">
        <template slot="iconImg">
          <i class="el-icon-s-order"></i>
        </template>
      </el-step>
      <el-step title="步骤 3" description="这段就没那么长了">
        <template slot="iconImg">
          <i class="el-icon-s-marketing"></i>
        </template>
      </el-step>
    </el-steps>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        input: 'Hello Element UI!'
      };
    }
  };
</script>
