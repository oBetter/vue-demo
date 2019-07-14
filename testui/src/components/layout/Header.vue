<template>
	<div class="header">
		<a href="/#/" class="logo">LOGO</a>
		<div class="nav">
			<router-link to="/">Home</router-link> |
			<router-link to="/about">About</router-link>
		</div>
		<div class="user"></div>
	</div>
</template>

<script>
export default {
	components: {},
	data() {
		return {};
	}
};
</script>

<style scoped lang='less'>
@import "./css/header.less";
</style>
