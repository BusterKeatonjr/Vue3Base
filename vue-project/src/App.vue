<script>
export default {
	data() {
		return {
     text:'aboba',
     visible: true, 
     visible1: false,
		}
},

}


</script>
<template>
<p v-if="visible">text</p>
<p v-if="visible1">text</p>
</template>

