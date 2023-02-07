<script>
export default {
	data() {
		return {
     text:'aboba',
     visible: true, 
     
		}
},

}


</script>
<template>
<p v-if="visible">text</p>
<p v-if="!visible">text</p>
</template>

