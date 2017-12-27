<template>
  <div style="display: flex;justify-content: space-between;max-width: 80%;">
    <div id="logo">
      hhhh
    </div>
    <div>
      <el-tabs v-model="activeName" @tab-click="handleClick">
      <el-tab-pane label="用户管理" name="first">用户管理1</el-tab-pane>
      <el-tab-pane label="配置管理" name="second">配置管理2</el-tab-pane>
      <el-tab-pane label="角色管理" name="third">角色管理3</el-tab-pane>
      <el-tab-pane label="定时任务补偿" name="fourth">定时任务补偿4</el-tab-pane>
    </el-tabs>
    </div>
  </div>


</template>

<script>
import { mapMutations } from 'vuex'
export default {
	data () {
		return {
      activeName: 'second'
		}
	},
	components: {
	},
	methods: {
		...mapMutations([
		  'pushLoadStack',
		  'completeLoad'
		]),
    handleClick(tab, event) {
      console.log(tab, event);
    }
	},
	created () {
	}
}
</script>

<style>

</style>

