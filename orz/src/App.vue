<template>
	<div id="app">
		<Header />
		<router-view />
		<Footer />
	</div>
</template>

<script>
import Header from '@/components/layout/Header'
import Footer from '@/components/layout/Footer'
export default {
	components: {
		Header,
		Footer
	}
}
</script>


<style lang="less">
@import './assets/css/common.less';
</style>
