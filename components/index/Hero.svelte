<main>
	<div>
		<section>
			<h1 class="size-lg brand-md" style:padding-bottom="4px">
				Hi, I'm Mike ✌️
			</h1>
			<p class="size-sm">
				I'm a frontend engineer and UI/UX designer based in Los Angeles, CA
			</p>
		</section>

		<ul>
			<li>
				<a
					href="mailto:mike@mikeploythai.com"
					target="_blank"
					rel="noopener noreferrer"
				>
					<ion-icon name="mail-outline" />
				</a>
			</li>
			|
			<li>
				<a
					href="https://github.com/mikeploythai"
					target="_blank"
					rel="noopener noreferrer"
				>
					<ion-icon name="logo-github" />
				</a>
			</li>
			<li>
				<a href="/youtube" target="_blank" rel="noopener noreferrer">
					<ion-icon name="logo-youtube" />
				</a>
			</li>
			<li>
				<a
					href="https://instagram.com/mikeploythai"
					target="_blank"
					rel="noopener noreferrer"
				>
					<ion-icon name="logo-instagram" />
				</a>
			</li>
		</ul>
	</div>
</main>

<style lang="scss">
	main {
		display: flex;
		align-items: center;
		justify-content: center;
		background-color: var(--navy-blue);
		min-height: 500px;

		div {
			display: flex;
			flex-direction: column;
			gap: 32px;
			width: 1200px;
			margin: 0 32px;

			ul {
				display: flex;
				gap: 16px;
				user-select: none;
			}

			a {
				display: flex;
				align-items: center;

				ion-icon {
					font-size: 24px;
				}
			}
		}
	}
</style>
