<template>
	<div class="container">
		<h3>Gelen Veriler</h3>
		<ul style="list-style-type:none;" class="list-group">
			<li v-for ="data in dataList" class="list-group-item">
				{{data}}
			</li>
		</ul>
	</div>
</template>

<script>
	export default {
		props  :{
			dataList : {
				required : false,
				type : Object

			}
		}
	}
</script>

