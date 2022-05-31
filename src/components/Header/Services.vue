<template>
	<div class="services">
		<ul class="services__list">
			<li class="services__item" v-for="item in servicesItems" :key="item">
				<a class="services__link" href="#"> {{ item }}</a>
			</li>
		</ul>
	</div>
</template>

<script>
export default {
	data() {
		return {
			servicesItems: [
				"Продвижение сайтов",
				"Создание сайтов",
				"Контекстная реклама",
			],
		};
	},
};
</script>

<style>
.services {
	background-color: #333333;
	padding: 8px 0;
}
.services__list {
	display: flex;
	justify-content: center;
}
.services__item {
	margin-right: 56px;
}
.services__item:last-child {
	margin-right: 0;
}
.services__link {
	font-family: "Fira Sans Extra Condensed";
	font-style: normal;
	font-weight: 500;
	font-size: 14px;
	line-height: 150%;
	text-transform: uppercase;
	color: #ffffff;
	text-decoration: none;
}
</style>