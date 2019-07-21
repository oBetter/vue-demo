<template>
	<div class="header">
		<router-link to="/" class="logo">LOGO</router-link>
		<el-menu :default-active="activeIndex" class="el-menu-demo" mode="horizontal" @select="handleSelect" background-color="#242329" text-color="#fff" active-text-color="#ffd04b" router>
			<el-menu-item index="/">Home</el-menu-item>
			<el-menu-item index="/about">About</el-menu-item>
			<el-submenu index="3">
				<template slot="title">我的工作台</template>
				<el-menu-item index="2-1">选项1</el-menu-item>
				<el-menu-item index="2-2">选项2</el-menu-item>
				<el-menu-item index="2-3">选项3</el-menu-item>
			</el-submenu>
		</el-menu>
		<div class="user"></div>
	</div>
</template>

<script>
export default {
	components: {},
	data() {
		return {
			activeIndex: '/'
		}
	},
	methods: {
		handleSelect(key, keyPath) {
			console.log(key, keyPath)
		}
	}
}
</script>

<style scoped lang='less'>
@import './css/header.less';
</style>
