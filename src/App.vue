<template>
	<NavBar />
	<NewsContent />
	<NewsFooter />
</template>

<script>
import NavBar from './components/NavBar.vue'
import NewsContent from './components/NewsContent.vue'
import NewsFooter from './components/NewsFooter.vue'

export default {
	components: {
		NavBar,
		NewsContent,
		NewsFooter,
	},
}
</script>

<style>
* {
	margin: 0;
	padding: 0;
	box-sizing: border-box;
	font-family: 'Roboto';
}
a {
	text-decoration: none;
}
li {
	list-style: none;
}
input,
button {
	background: none;
	outline: none;
	border: none;
	transition: 0.5s;
}
button:active {
	transform: scale(0.95);
}
.container {
	width: 100%;
	max-width: 1140px;
	padding: 0 15px;
	margin: 0 auto;
}
</style>
