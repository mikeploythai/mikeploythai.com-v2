<script lang="ts">
	const project = [
		{
			title: "ACM Chapter at CSUF Website",
			link: "https://github.com/ethanthatonekid/acmcsuf.com",
			img: "photos/acm-website.png",
		},
		{
			title: "TuffyHacks 2022 Website",
			link: "https://tuffyhacks.com",
			img: "photos/th-website.png",
		},
	];
</script>

<main>
	<div>
		<h1 class="size-md brand-md">Featured Projects</h1>

		<section>
			{#each project as { title, link, img } (link)}
				<a
					href={link}
					target="_blank"
					rel="noopenner noreferrer"
					style:background-image="url({img})"
				>
					<h2 class="size-sm brand-md">{@html title}</h2>
				</a>
			{/each}
		</section>
	</div>
</main>

<style lang="scss">
	main {
		display: flex;
		align-items: center;
		justify-content: center;

		div {
			display: flex;
			flex-direction: column;
			gap: 32px;
			width: 1200px;
			margin: 0 32px;

			h1 {
				color: var(--navy-blue);
			}

			section {
				display: grid;
				width: 100%;
				grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
				gap: 32px;

				a {
					display: flex;
					align-items: center;
					justify-content: center;
					justify-items: stretch;
					height: 250px;
					border-radius: 20px;
					background-color: var(--navy-blue);
					background-size: cover;
					background-position: top center;
					transition: 0.25s ease-in-out;

					h2 {
						opacity: 0;
						color: var(--highlight-blue);
						transition: 0.25s ease-in-out;
					}

					&:hover {
						box-shadow: inset 0 0 0 2000px rgba(var(--navy-rgb), 0.75);
						filter: drop-shadow(0 4.5px 22.5px rgba(var(--navy-rgb), 0.75));

						h2 {
							opacity: 1;
						}
					}
				}
			}
		}
	}
</style>
