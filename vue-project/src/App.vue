<script>
export default {
	data() {
		return {
			
		}
},
methods: {
	show: function() {
    const current = new Date();
    const date = `${current.getDate()}/${current.getMonth() + 1}/${current.getFullYear()}`;
    alert(date);
	}
}
}
</script>
<template>
  <button @click="show">text</button> <br>
	<button @mouseenter="show">text</button>
</template>

