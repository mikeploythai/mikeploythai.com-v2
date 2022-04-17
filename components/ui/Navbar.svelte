<nav>
	<div>
		<a href="#" class="size-md brand-md">MP</a>

		<a
			href="/resume.pdf"
			class="size-sm button"
			target="_blank"
			rel="noopenner noreferrer"
		>
			Resume
		</a>
	</div>
</nav>

<style lang="scss">
	nav {
		display: flex;
		position: fixed;
		z-index: 10;
		justify-content: center;
		align-items: center;
		width: 100%;
		padding: 24px 0;
		background-color: var(--navy-blue);

		div {
			display: flex;
			justify-content: space-between;
			align-items: center;
			width: 1200px;
			margin: 0 32px;

			.button {
				padding: 8px 12px;
				border: 2px solid var(--baby-blue);
				border-radius: 6px;

				&:hover {
					border: 2px solid var(--highlight-blue);
				}
			}
		}
	}
</style>
