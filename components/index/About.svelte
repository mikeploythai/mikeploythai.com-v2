<main>
	<div>
		<section>
			<h1 class="size-md brand-md" style:padding-bottom="4px">About Me</h1>
			<p>
				I'm a third year university student studying computer science with deep
				interests in building and designing beautiful applications for the web.
				<br /><br />
				I've always considered myself a creator more than anything. I love to express
				my ideas through various mediums like videography and music, and being a
				frontend software engineer allows me to do that whilst bridging the gap between
				my passions for creativity and tech. My goal is to build rich experiences
				for people through web and mobile technologies that improve their relationship
				with tech.
				<br /><br />
				When I'm not designing or developing cool things, I'm probably working on
				my YouTube content, playing my guitar, or hanging out with family/friends.
				<br /><br />
				Currently the Create Path President in the ACM Chapter at CSUF.
			</p>
		</section>

		<img src="photos/mike.jpg" alt="Photo of Mike" />
	</div>
</main>

<style lang="scss">
	main {
		display: flex;
		align-items: center;
		justify-content: center;

		div {
			display: flex;
			align-items: center;
			justify-content: space-between;
			width: 1200px;
			margin: 0 32px;

			section {
				max-width: 600px;

				h1,
				p {
					color: var(--navy-blue);
				}
			}

			img {
				aspect-ratio: 1/1;
				height: auto;
				min-width: 250px;
				max-width: 320px;
				width: 100%;
				margin-left: 32px;
				border-radius: 20px;
				object-fit: cover;
				object-position: 0 30%;
			}
		}
	}

	@media screen and (max-width: 768px) {
		main div {
			flex-direction: column-reverse;
			align-items: flex-start;
			gap: 32px;

			img {
				margin-left: 0;
			}
		}
	}
</style>
