<template>
	<main class="main">
		<section class="news">
			<div class="news__content">
				<div class="news__content-item">
					<img src="@/assets/images/Preview-1.png" alt="" />
					<h2 class="news__content-item-title">
						A Midwestern capital is marching for racial justice — and getting
						results
					</h2>
					<p class="news__content-item-descr">
						Outside of the governor’s mansion in Des Moines, Iowa, on Tuesday
						evening, Dionna Langford spoke to a crowd of hundreds of protesters
						with a bullhorn. “Black people,” said Langford, 28, who is African
						American, “if you have been harassed, terrorized, bullied by the
						police, in this city, make some...
					</p>
				</div>
				<div class="news__content-item-2">
					<h2 class="news__content-item-title">
						A Midwestern capital is marching for racial justice — and getting
						results
					</h2>
					<p class="news__content-item-descr">
						Outside of the governor’s mansion in Des Moines, Iowa, on Tuesday
						evening, Dionna Langford spoke to a crowd of hundreds of protesters
						with a bullhorn. “Black people,” said Langford, 28, who is African
						American, “if you have been harassed, terrorized, bullied by the
						police, in this city, make some...
					</p>
					<img src="@/assets/images/Preview-2.png" alt="" />
				</div>
				<div class="news__content-item-3">
					<img src="@/assets/images/Preview-3.png" alt="" />
					<h2 class="news__content-item-title">
						A Midwestern capital is marching for racial justice — and getting
						results
					</h2>
					<p class="news__content-item-descr">
						Outside of the governor’s mansion in Des Moines, Iowa, on Tuesday
						evening, Dionna Langford spoke to a crowd of hundreds of protesters
						with a bullhorn. “Black people,” said Langford, 28, who is African
						American, “if you have been harassed, terrorized, bullied by the
						police, in this city, make some...
					</p>
				</div>
				<div class="news__content-item-4">
					<h2 class="news__content-item-title">
						A Midwestern capital is marching for racial justice — and getting
						results
					</h2>
					<p class="news__content-item-descr">
						Outside of the governor’s mansion in Des Moines, Iowa, on Tuesday
						evening, Dionna Langford spoke to a crowd of hundreds of protesters
						with a bullhorn. “Black people,” said Langford, 28, who is African
						American, “if you have been harassed, terrorized, bullied by the
						police, in this city, make some...
					</p>
					<img src="@/assets/images/Preview-4.png" alt="" />
				</div>
			</div>
			<h1 class="news__content-bottom-title">Главные новости</h1>
		</section>
	</main>
	<MainNews />
</template>

<script>
import MainNews from '@/components/MainNews.vue'
export default {
	components: {
		MainNews,
	},
}
</script>

<style>
.news__content {
	display: flex;
	align-items: center;
	justify-content: center;
}

.news__content-item {
	display: flex;
	flex-direction: column;
	align-items: start;
	background-color: red;
	max-width: min-content;
}
.news__content-item:hover,
.news__content-item-2:hover,
.news__content-item-3:hover,
.news__content-item-4:hover {
  background: black;
  transition: 0.7s;
}
.news__content-item-2 {
	display: flex;
	flex-direction: column;
	background: rgb(106, 27, 154);
	max-width: min-content;
}
.news__content-item-3 {
	display: flex;
	flex-direction: column;
	background: rgb(48, 63, 159);
	max-width: min-content;
}
.news__content-item-4 {
	display: flex;
	flex-direction: column;
	background: rgb(0, 105, 92);
	max-width: min-content;
}

.news__content-item-title {
	padding-left: 15px;
	color: rgb(255, 255, 255);
	font-size: 19px;
	font-weight: 700;
	line-height: 22px;
	margin-top: 8px;
}
.news__content-item-descr {
	padding-left: 15px;
	margin-top: 8px;
	margin-bottom: 15px;
	color: rgb(235, 235, 235);
	font-size: 16px;
	font-weight: 400;
	line-height: 19px;
}
.news__content-bottom-title {
	margin-top: 40px;
	text-align: center;
	color: rgb(58, 56, 56);
	font-size: 22px;
	font-weight: 700;
	line-height: 26px;
	margin-bottom: 40px;
}
</style>
