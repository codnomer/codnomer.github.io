<script>
	let greeting = 'Step Into the Digital Realm';
	let welcomeMessage =
		'Where Code Meets Creativity - I’m Omer Demirhan, crafting ideas into impactful solutions.';
	let callToAction = 'Explore My Work';
	let aboutLink = '/about';
	let blogLink = '/blog';
	let ideasLink = '/ideas';
</script>

<main class="welcome-page">
	<section class="hero">
		<div class="hero-content">
			<h1 class="fade-in">{greeting}</h1>
			<p class="fade-in-delay">{welcomeMessage}</p>
			<a href={aboutLink} class="cta bounce">{callToAction}</a>
		</div>
	</section>

	<section class="explore-section">
		<h2 class="fade-in">Explore More</h2>
		<div class="explore-cards">
			<div class="card blog-card scale-up">
				<h3>Blog</h3>
				<p>Dive deep into my thoughts on coding, AI, and tech trends.</p>
				<a href={blogLink} class="cta">Visit Blog</a>
			</div>

			<div class="card ideas-card scale-up">
				<h3>Ideas</h3>
				<p>Discover my creative ideas and projects in progress.</p>
				<a href={ideasLink} class="cta">Explore Ideas</a>
			</div>
		</div>
	</section>

	<section class="animation-bg">
		<div class="wave"></div>
		<div class="wave wave2"></div>
		<div class="wave wave3"></div>
	</section>
</main>

<style>
	/* Reset */
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
	}

	body {
		font-family: 'Montserrat', sans-serif;
		background-color: #f4f4f4;
		color: #333;
		overflow-x: hidden;
	}

	a {
		text-decoration: none;
		color: inherit;
	}

	/* Hero Section */
	.hero {
		height: 100vh;
		display: flex;
		align-items: center;
		justify-content: center;
		text-align: center;
		background-color: #007acc;
		color: white;
		overflow: hidden;
		position: relative;
	}

	.hero-content {
		position: relative;
		z-index: 1;
	}

	h1 {
		font-size: 4.5rem;
		font-weight: 800;
		line-height: 1.2;
		margin-bottom: 20px;
		color: white;
	}

	p {
		font-size: 1.5rem;
		margin-bottom: 30px;
		max-width: 600px;
		color: #f0f0f0;
	}

	.cta {
		background-color: white;
		color: #007acc;
		padding: 15px 30px;
		font-size: 1.2rem;
		border-radius: 30px;
		transition:
			background-color 0.3s ease,
			transform 0.3s ease;
	}

	.cta:hover {
		background-color: #00d1b2;
		color: white;
		transform: scale(1.1);
	}

	/* Explore Section */
	.explore-section {
		padding: 60px 20px;
		text-align: center;
	}

	.explore-section h2 {
		font-size: 2.5rem;
		margin-bottom: 30px;
		animation: fadeIn 2s ease-in;
	}

	.explore-cards {
		display: grid;
		grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
		gap: 20px;
		max-width: 1000px;
		margin: 0 auto;
	}

	.card {
		background-color: white;
		padding: 40px;
		border-radius: 20px;
		box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
		transition: transform 0.3s ease;
	}

	.card:hover {
		transform: translateY(-10px);
	}

	.card h3 {
		font-size: 2rem;
		color: #007acc;
	}

	.card p {
		margin: 20px 0;
		font-size: 1.1rem;
		color: #555;
	}

	/* Waves for background effect */
	.animation-bg {
		position: absolute;
		bottom: 0;
		left: 0;
		right: 0;
		height: 300px;
		z-index: 0;
		overflow: hidden;
	}

	.wave {
		position: absolute;
		width: 200%;
		height: 100%;
		background: rgba(255, 255, 255, 0.2);
		opacity: 0.5;
		border-radius: 40%;
		animation: wave 6s infinite linear;
	}

	.wave2 {
		animation-duration: 8s;
		background: rgba(255, 255, 255, 0.3);
	}

	.wave3 {
		animation-duration: 10s;
		background: rgba(255, 255, 255, 0.4);
	}

	@keyframes wave {
		0% {
			transform: translateX(-50%);
		}
		100% {
			transform: translateX(50%);
		}
	}

	/* Animations */
	@keyframes fadeIn {
		0% {
			opacity: 0;
			transform: translateY(20px);
		}
		100% {
			opacity: 1;
			transform: translateY(0);
		}
	}

	.fade-in {
		animation: fadeIn 1.5s ease-out;
	}

	.fade-in-delay {
		animation: fadeIn 2s ease-out;
	}

	.bounce {
		animation: bounce 2s infinite;
	}

	@keyframes bounce {
		0%,
		100% {
			transform: translateY(0);
		}
		50% {
			transform: translateY(-10px);
		}
	}
</style>
