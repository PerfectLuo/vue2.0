<template>
	<div>
		<Header></Header>
		<div class="artice_list">
			
		</div>
		<Footer></Footer>
	</div>
</template>
<script>
import Header from "../components/header.vue"
import Footer from "../components/footer.vue"

	export default {
		components:{Header,Footer},

		created(){
			this.$api.get('topics',null,r=>{
				console.log(r)
			})
		}
	}
</script>