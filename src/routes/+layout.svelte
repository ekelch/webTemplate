<script lang="ts">
	let { children } = $props();
</script>

<nav id="nav-outer">
	<div id="nav-inner">
		<a href="/">Home</a>
		<a href="/about">About</a>
	</div>
</nav>

{@render children()}

<style lang="css">
    :global(body) {
        margin: 0;
        font-family: "Palatino Linotype", serif;
        font-size: 16px;
				background: #DBD3C9;
    }

    #nav-outer {
				display: flex;
    }

    #nav-inner {
        height: 40px;

        display: flex;
        gap: 12px;
        margin: 12px auto 16px;
        padding: 0;
    }


    #nav-inner a {
        padding: 0 16px;
        align-content: center;
        text-decoration: none;
        background: rgba(0, 0, 0, 0.05);
        border-radius: 12px;


    }

    #nav-inner a:hover {
        background: rgba(0, 0, 0, 0.08);
    }
</style>