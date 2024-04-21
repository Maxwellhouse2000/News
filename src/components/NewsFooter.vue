<template>
	<footer class="footer">
		<div class="container footer__content">
			<a href="" class="footer__logo">
				<img src="@/assets/images/footer__logo.png" alt="" />
				THE NEWS WEB
			</a>
			<ul class="footer__list">
				<li>
					<a class="footer__list-link" href=""><span>СПЕЦПРОЕКТ</span></a>
				</li>
				<li v-for="(link, i) in links" :key="i">
					<a href="#" class="footer__list-link">
						{{ link.name }}
					</a>
				</li>
			</ul>
		</div>
	</footer>
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
.footer {
	margin-top: 50px;
	background: rgb(58, 56, 56);
	padding: 28px 54px;
}
.footer__content {
	display: flex;
    align-items: center;
    justify-content: space-between;
}
.footer__logo {
	display: flex;
	flex-direction: column;
	align-items: center;
	color: rgb(255, 255, 255);
	font-size: 18px;
	font-weight: 700;
	line-height: 21px;
}
.footer__list {
	display: flex;
	gap: 15px;
}
.footer__list-link {
	color: rgb(255, 255, 255);
	font-size: 18px;
	font-weight: 700;
	line-height: 21px;
}
.footer__list-link:hover {
	color: rgb(239, 68, 35);
	text-decoration: underline;
}
.footer__list-link span {
	color: rgb(239, 68, 35);
	font-size: 18px;
	font-weight: 700;
	line-height: 21px;
}
</style>
