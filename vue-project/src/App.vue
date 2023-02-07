<script>
export default {
	data() {
		return {
      num2: 2,
      num3: 3,
		}
},
methods: {
	show: function() {
    alert(this.num2 * 2); 

     
	},
  bob: function(){
    alert(this.num3 * 3); 
  }
}
}
</script>
<template>

<button @click="show">btn1</button>
	<button @click="bob">btn2</button>
</template>

