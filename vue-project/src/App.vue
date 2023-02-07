<script>
export default {
	data() {
		return {
     text:'abiba',
      url:'https://code.mu/ru/javascript/framework/vue/book/prime/basis/events-modifiers/',
		}
},
methods: {
    warning: function(){
      alert('one click');
    }
}
}

</script>
<template>
 <a @click.prevent :href=url>{{ text }}</a> <br>
 <button @click.once="warning"> click </button>
</template>

