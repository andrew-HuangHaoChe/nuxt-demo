<script setup>
const {data} = await useFetch("https://60bd9841ace4d50017aab3ec.mockapi.io/api/post_card")

onMounted(() => {
})
</script>
<template>
    <h1>首頁</h1>
	<ul>
		<li v-for="item in data" :key="item.id">
			<img :src="item.avatar" alt="">
			<p>createdAt:{{ item.createdAt }}</p>
			<p>name:{{ item.name }}</p>
			<p>post_date: {{ item.post_date }}</p>
			<p>content: {{ item.content }}</p>
		</li>
	</ul>
</template>