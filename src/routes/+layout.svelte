<script lang="ts">
	let {children} = $props();
</script>

<nav>
	<a href="/">home</a>
	<a href="/about">about</a>
</nav>

{@render children()}

<style lang="css">
		:global(body) {
				margin: 0;
		}

	nav {
			width: 100%;
			height: 40px;
			background: darkgreen;

			display: flex;
			gap: 8px;
			margin: 0;
			padding: 0;
	}

	nav a {
			margin: 6px 0;
			padding: 0 12px;
			align-content: center;
			border-radius: 4px;
			text-decoration: none;
	}

	nav a:hover {
			background: darkgrey;
	}
</style>