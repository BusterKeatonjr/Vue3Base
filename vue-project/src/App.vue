<script>
export default {
	data() {
		return {
			arr: ['x', 'y', 'z', 1, 2, 3],
		}
	}
}
</script>
<template>
	{{ arr[0] }} <br>
	{{ arr[1] }} <br>
	{{ arr[2] }} <br>
  {{ arr[3] + arr[4] + arr[5] }}
</template>

