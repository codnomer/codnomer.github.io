<script>
	let ideas = [
		{
			title: 'AI-Powered Mood Detection',
			description:
				'Using machine learning to detect emotional states based on text inputs and facial expressions.',
			status: 'Completed'
		},
		{
			title: 'Educational Platform According to Learning Style',
			description: 'Building AI-based educational tools to enhance student learning experiences.',
			status: 'Concept Stage'
		}
	];
</script>

<main class="ideas-page">
	<section class="ideas-header">
		<h1 class="fade-in">Ideas in the Dark</h1>
		<p class="fade-in-delay">
			Where innovation meets possibility. Here are a few projects and concepts I'm exploring in the
			realms of AI, Database, 6G, and more.
		</p>
	</section>

	<section class="ideas-list">
		{#each ideas as idea}
			<div class="idea-card fade-in-delay">
				<h2>{idea.title}</h2>
				<p>{idea.description}</p>
				<div class="status">{idea.status}</div>
			</div>
		{/each}
	</section>
</main>

<style>
	/* Dark theme background */
	main {
		font-family: 'Montserrat', sans-serif;
		background-color: #121212;
		color: #f0f0f0;
		margin: 0;
		padding: 0;
		overflow-x: hidden;
	}

	/* Header */
	.ideas-header {
		text-align: center;
		padding: 80px 20px;
		color: #00d1b2;
	}

	.ideas-header h1 {
		font-size: 4rem;
		font-weight: bold;
	}

	.ideas-header p {
		font-size: 1.3rem;
		max-width: 800px;
		margin: 20px auto;
	}

	/* Ideas List */
	.ideas-list {
		display: grid;
		grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
		gap: 20px;
		max-width: 1200px;
		margin: 0 auto;
		padding: 40px 20px;
	}

	/* Idea Card */
	.idea-card {
		background: rgba(255, 255, 255, 0.05);
		padding: 40px;
		border-radius: 15px;
		box-shadow: 0 4px 20px rgba(0, 0, 0, 0.5);
		transition:
			transform 0.3s ease,
			box-shadow 0.3s ease;
		position: relative;
		overflow: hidden;
	}

	.idea-card:hover {
		transform: translateY(-10px);
		box-shadow: 0 6px 30px rgba(0, 0, 0, 0.7);
	}

	.idea-card h2 {
		font-size: 2rem;
		color: #00d1b2;
	}

	.idea-card p {
		margin: 20px 0;
		font-size: 1.1rem;
		line-height: 1.6;
	}

	.status {
		font-size: 0.9rem;
		color: #00d1b2;
		background: rgba(255, 255, 255, 0.1);
		padding: 5px 15px;
		border-radius: 20px;
		width: fit-content;
		margin-top: 10px;
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
</style>
