<template>
  <div style="display: flex;flex-direction: column;text-align: center;">
    <div>
      <div style="text-align: center;margin: 20px 0;">
        <el-button type="primary" plain>热门</el-button>
        <el-button type="primary" plain>最新</el-button>
        <el-button type="primary" plain>我的</el-button>
      </div>
      <div>
        hhhhhh
      </div>
    </div>
  </div>


</template>

<script>
import { mapMutations } from 'vuex'
export default {
	data () {
		return {
		}
	},
	components: {
	},
	methods: {
		...mapMutations([
		  'pushLoadStack',
		  'completeLoad'
		])
	},
	created () {
	}
}
</script>

<style>
  .bg-purple {
    background: #d3dce6;
  }
  .grid-content {
    border-radius: 4px;
    min-height: 36px;
  }
</style>

