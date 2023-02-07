<script>
export default {
	data() {
		return {
      text: 'xxx',
		}
},
methods: {
	change: function() {
		this.text = 'yyy';
},
change1: function() {
		this.text = 'aaa';
	}

}
}
</script>
<template>
{{ text }} <br>
<button @click="change" >switch1</button><br>
<button @click="change1" >switch2</button> 
</template>

