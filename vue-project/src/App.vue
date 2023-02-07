<script>
export default {
	data() {
		return {
      cost: 10,
      amount:4,
		}
},
computed: {
	price: function() {
		return this.cost * this.amount;
	},
  change: function(){
    this.cost = 8
  }
}
}
</script>
<template>
 {{ price }} <br>
 <button @click="change">swich</button>
</template>

