<template>
	<div class="header">
		<router-link to="/" class="logo">LOGO</router-link>
		<el-menu :default-active="activeIndex" class="el_menu" mode="horizontal" @select="handleSelect" background-color="#242329" text-color="#fff" active-text-color="#ffd04b" router>
			<el-menu-item index="/">Home</el-menu-item>
			<el-menu-item index="/about">About</el-menu-item>
			<el-submenu index="" class="user">
				<template slot="title">pwx609952</template>
				<el-menu-item index="/personalCenter">个人中心</el-menu-item>
				<el-menu-item index="" @click="loginOut">注销</el-menu-item>
			</el-submenu>
		</el-menu>
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
		// 注销
		loginOut() {

		},
		// 选中的菜单
		handleSelect(key, keyPath) {
			console.log(key, keyPath)
		}
	}
}
</script>

<style scoped lang='less'>
@import './css/header.less';
</style>
