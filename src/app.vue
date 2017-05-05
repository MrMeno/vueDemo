<template>
  <div>
    <h1>element-cooking-starter</h1>
    <p>Use Vue 2.0 Today!</p>
    <el-button @click.native="startHacking">Let's do it</el-button>
      <el-radio class="radio" v-model="radio" label="1">备选项</el-radio>
  <el-radio class="radio" v-model="radio" label="2">备选项</el-radio>

   <el-submenu index="2">
    <template slot="title">我的工作台</template>
    <el-menu-item index="2-1">选项1</el-menu-item>
    <el-menu-item index="2-2">选项2</el-menu-item>
    <el-menu-item index="2-3">选项3</el-menu-item>
  </el-submenu>
  </div>
</template>

<script>
  export default {
    name: 'app',

    methods: {
      startHacking() {
        this.$notify({
          title: 'It Works',
          message: 'We have laid the groundwork for you. Now it\'s your time to build something epic!',
          duration: 6000
        });
      }
    }
  };
</script>
<style>
  .radio{

  }
</style>
