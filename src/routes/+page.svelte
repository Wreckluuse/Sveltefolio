<script>
	import Navigation from '$lib/Navigation.svelte';
</script>

<svelte:head>
	<title>Portfolio</title>
</svelte:head>
<body>
	<Navigation />
</body>

<style>
	body {
		position: fixed;
		top: 0;
		left: 0;
		margin: 0;
		height: 100vh;
		width: 100vw;
		background: hsla(212, 45%, 45%, 1);

		background: linear-gradient(
			90deg,
			hsla(212, 45%, 45%, 1) 0%,
			hsla(212, 51%, 42%, 1) 26%,
			hsla(0, 0%, 100%, 1) 100%
		);

		background: -moz-linear-gradient(
			90deg,
			hsla(212, 45%, 45%, 1) 0%,
			hsla(212, 51%, 42%, 1) 26%,
			hsla(0, 0%, 100%, 1) 100%
		);

		background: -webkit-linear-gradient(
			90deg,
			hsla(212, 45%, 45%, 1) 0%,
			hsla(212, 51%, 42%, 1) 26%,
			hsla(0, 0%, 100%, 1) 100%
		);
	}
</style>
