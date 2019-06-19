<template>
	<div class="navbar navbar-default topnav">
		<div class="container">
			<div class="navbar-hander">
				<a href="#" class="navbar-brand">
					<span class="title">{{ logo.title }}</span>
					<img :src="logo.src" :alt="logo.title">
				</a>
			</div>
		</div>
	</div>
</template>

<script>
export default {
	name: 'TheHeader',
	data() {
		return {
			logo: {
				src:`${this.uploadsUrl}sites/ByvFbNlQYVwhvTyBgLdqitchoacDNznN.jpg`,
				title: 'VueCaff'
			}
		}
	},
	beforeCreate() {
		this.uploadsUrl = 'https://vuejscaffcdn.phphub.org/uploads/'
	}
}
</script>

<style scoped>
	.title { display:none;}
</style>
