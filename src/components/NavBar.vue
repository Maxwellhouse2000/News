<template>
	<nav class="nav">
		<div class="container nav__content">
			<a href="#" class="nav__logo"
				><img src="@/assets/images/Header-h1.png" alt="" />
				THE NEWS WEB
			</a>
			<ul class="nav__list">
				<li>
					<a class="nav__list-link" href=""><span>СПЕЦПРОЕКТ</span></a>
				</li>
				<li v-for="(link, i) in links" :key="i">
					<a href="#" class="nav__list-link">
						{{ link.name }}
					</a>
				</li>
			</ul>
		</div>
	</nav>
	<img src="@/assets/images/Header-background.jpg" alt="" />
</template>

<script>
export default {
	data() {
		return {
			links: [
				{ name: 'ОБЩЕСТВО ', to: 'ОБЩЕСТВО ' },
				{ name: 'ТЕХНОЛОГИИ', to: 'ТЕХНОЛОГИИ' },
				{ name: 'ЭКОНОМИКА', to: 'ЭКОНОМИКА' },
				{ name: ' ПОЛИТИКА ', to: ' ПОЛИТИКА ' },
				{ name: ' СПОРТ ', to: ' СПОРТ ' },
			],
		}
	},
	
}
</script>

<style>
.nav {
	padding: 23px 0;
}
.nav__logo {
	display: flex;
	flex-direction: column;
	align-items: center;
	color: rgb(0, 0, 0);
	font-size: 18px;
	font-weight: 700;
	line-height: 21px;
}
.nav__content {
	display: flex;
	align-items: center;
	justify-content: space-between;
}
.nav__list {
	display: flex;
	gap: 15px;
}
.nav__list-link {
	color: rgb(58, 56, 56);
	font-size: 18px;
	font-weight: 700;
	line-height: 21px;
}
.nav__list-link:hover {
	color: rgb(239, 68, 35);
	text-decoration: underline;
}
.nav__list-link span {
	color: rgb(239, 68, 35);
	font-size: 18px;
	font-weight: 700;
	line-height: 21px;
}
</style>
