<script>
	const navItems = [
		{ name: 'Games', href: '/Games', live: true },
		{ name: 'Software', href: '/Software', live: true },
		{ name: 'Music', href: '/Music', live: false },
		{ name: 'eSports', href: '/eSports', live: true },
		{ name: 'Literature', href: '/Literature', live: false }
	];
</script>

<nav class="navbar">
	<div class="navbar-container">
		<div class="navbar-logo">
			<a href="/">Remember the Ravens</a>
		</div>

		<div class="navbar-menu">
			{#each navItems as item}
				{#if item.live}
					<a href={item.href} class="navbar-item">{item.name}</a>
				{:else}
					<span class="disabled">{item.name}</span>
				{/if}
			{/each}
		</div>
	</div>
</nav>

<style>
	nav {
		display: flex;
		gap: 1rem;
		background-color: #111;
		padding: 1rem;
		color: white;
	}

	a,
	span {
		position: relative;
		padding: 0.5rem 1rem;
		border-radius: 8px;
		text-decoration: none;
		font-weight: bold;
		transition: background 0.2s;
	}

	a:hover {
		background-color: #222;
	}

	.disabled {
		color: #888;
		cursor: default;
	}

	.disabled:hover::after {
		content: 'Coming soon';
		position: absolute;
		top: 100%;
		left: 0;
		background: #333;
		color: white;
		padding: 0.25rem 0.5rem;
		font-size: 0.8rem;
		border-radius: 4px;
		white-space: nowrap;
		margin-top: 0.3rem;
		z-index: 10;
	}
</style>
