<script lang="ts">
</script>

<svelte:head>
	<title>About - Ganesh</title>
</svelte:head>

<main>
	<div class="container">
		<header class="page-header">
			<h1>About Me</h1>
		</header>

		<div class="content">
			<div class="photo-container">
				<img src="/photo of me.jpg" alt="Ganesh" class="profile-photo" />
			</div>
			
			<div class="text-section">
				<p>
					Hi! I'm Ganesh, a high schooler from Bangalore, India. I love anything deep tech, programming and rocketry.
				</p>
				<p>
					I love beaches, HackClub and hanging out with my friends.
				</p>
				<p>
					Check out what I've done and what I'm up to on my <a href="/projects" style="color: rgb(176, 135, 255) !important;">projects page</a>.
				</p>
			</div>
		</div>
	</div>
</main>

<style>
	main {
		min-height: 100vh;
		padding: 100px 24px 80px;
		background: #f8f9fa;
	}

	.container {
		max-width: 800px;
		margin: 0 auto;
	}

	.page-header {
		text-align: center;
		margin-bottom: 48px;
	}

	.page-header h1 {
		font-size: 3rem;
		font-weight: 700;
		margin: 0;
		color: #000000;
	}

	.content {
		background: #ffffff;
		border: 2px solid #000000;
		border-radius: 16px;
		padding: 48px;
		box-shadow: 4px 4px 0px #000000;
		display: flex;
		gap: 40px;
		align-items: flex-start;
	}

	.photo-container {
		position: relative;
		flex-shrink: 0;
		width: 350px;
	}

	.profile-photo {
		width: 100%;
		height: auto;
		border: 3px solid #000000;
		box-shadow: 4px 4px 0px #000000;
		transition: all 0.3s ease;
		display: block;
	}

	.profile-photo:hover {
		transform: translate(-2px, -2px);
		box-shadow: 6px 6px 0px #000000;
	}

	.text-section {
		flex: 1;
		min-width: 0;
	}

	.text-section a {
		color: rgba(176, 135, 255, 1) !important;
		text-decoration: underline;
		text-underline-offset: 2px;
		font-weight: 600;
		transition: color 0.2s ease, text-decoration-thickness 0.2s ease;
	}

	.text-section a:link {
		color: rgba(176, 135, 255, 1) !important;
	}

	.text-section a:hover {
		color: rgba(23, 241, 209, 1) !important;
		text-decoration-thickness: 2px;
	}

	.text-section a:focus-visible {
		outline: 2px solid rgba(176, 135, 255, 1);
		outline-offset: 2px;
		border-radius: 2px;
	}

	.content p {
		font-size: 1.25rem;
		line-height: 1.8;
		color: #000000;
		margin: 0 0 24px 0;
		font-weight: 500;
	}

	.content p:last-child {
		margin-bottom: 0;
	}

	@media (max-width: 768px) {
		main {
			padding: 80px 20px 60px;
		}

		.page-header h1 {
			font-size: 2.5rem;
		}

		.content {
			padding: 32px 24px;
			flex-direction: column;
			gap: 24px;
		}

		.photo-container {
			width: 100%;
			max-width: 350px;
			margin: 0 auto;
		}

		.content p {
			font-size: 1.1rem;
		}
	}

	@media (max-width: 480px) {
		.page-header h1 {
			font-size: 2rem;
		}

		.content {
			padding: 24px 20px;
		}

		.photo-container {
			max-width: 100%;
		}

		.easter-egg {
			font-size: 0.85rem;
			padding: 16px;
		}

		.easter-egg p {
			font-size: 0.85rem;
		}

		.content p {
			font-size: 1rem;
		}
	}
</style>