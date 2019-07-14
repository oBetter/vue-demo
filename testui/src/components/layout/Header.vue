<template>
	<div class="header">
		<a href="/#/" class="logo">LOGO</a>
		<el-menu :default-active="activeIndex" class="el-menu-demo" mode="horizontal" @select="handleSelect" background-color="#24292e" text-color="#fff" active-text-color="#ffd04b">
			<el-menu-item index="1">
				<router-link to="/">Home</router-link>
			</el-menu-item>
			<el-menu-item index="2">
				<router-link to="/about">About</router-link>
			</el-menu-item>
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
			activeIndex: '1'
		}
	}
}
</script>

<style scoped lang='less'>
@import './css/header.less';
</style>
