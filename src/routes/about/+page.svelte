<script>
	let name = 'Omer Demirhan';
	let title = 'Full Stack Developer & AI Engineer';
	let tagline = 'Crafting Dynamic & Scalable Software Solutions';
	let skills = [
		'Full Stack Development',
		'Artificial Intelligence',
		'Database Management',
		'Server Management'
	];
	let projects = [
		{
			name: 'ERP Software',
			description: 'A flexible and scalable ERP system developed for Mepsan AS.',
			link: '#'
		},
		{
			name: 'AI Solutions',
			description: 'Deep learning models to optimize automation processes at Pusula.ai.',
			link: '#'
		},
		{
			name: 'Chatbot',
			description: 'An AI-driven chatbot to detect psychological moods.',
			link: '#'
		}
	];
	let contactLink = 'mailto:demirhanomer11@gmail.com';
</script>

<main class="landing-page">
	<section class="hero">
		<div class="hero-content">
			<h1 class="fade-in">{name}</h1>
			<h2 class="slide-up">{title}</h2>
			<p class="fade-in-delay">{tagline}</p>
			<a href="#projects" class="cta bounce">Explore My Work</a>
		</div>
	</section>

	<section class="about" id="about">
		<h2 class="slide-up">About Me</h2>
		<p class="fade-in">
			I'm <strong>{name}</strong>, a passionate <strong>{title}</strong> based in Izmir, Türkiye. With
			experience in both full stack development and artificial intelligence, I build dynamic and scalable
			software that solves real-world problems. I specialize in crafting robust applications using technologies
			like Node.js, Python, PostgreSQL, and more.
		</p>
		<p class="fade-in">
			Whether it’s developing ERP systems, implementing AI-driven solutions, or leading teams, I am
			always learning and evolving to deliver impactful software.
		</p>
	</section>

	<section class="skills" id="skills">
		<h2 class="slide-up">Skills</h2>
		<div class="skills-grid">
			{#each skills as skill}
				<div class="skill-card scale-up">
					<h3>{skill}</h3>
				</div>
			{/each}
		</div>
	</section>

	<section class="projects" id="projects">
		<h2 class="slide-up">Projects</h2>
		<div class="project-grid">
			{#each projects as project}
				<div class="project-card hover-raise">
					<h3>{project.name}</h3>
					<p>{project.description}</p>
					<a href={project.link} target="_blank">View Project</a>
				</div>
			{/each}
		</div>
	</section>

	<section class="contact" id="contact">
		<h2 class="fade-in">Contact Me</h2>
		<p class="fade-in">
			If you'd like to discuss a project or just say hello, feel free to reach out!
		</p>
		<a href={contactLink} class="contact-btn bounce">Get In Touch</a>
	</section>
</main>

<style>
	/* Basic Reset */
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
	}

	body {
		font-family: 'Montserrat', sans-serif;
		background-color: #f4f4f4;
		color: #333;
		scroll-behavior: smooth;
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
		background: linear-gradient(135deg, #d8dee2 0%, #bde6e0 100%);
		color: rgb(11, 10, 10);
		overflow: hidden;
	}

	.hero-content {
		text-align: center;
	}

	h1 {
		font-size: 4rem;
		font-weight: 900;
	}

	h2 {
		font-size: 2rem;
		margin-top: 10px;
	}

	p {
		font-size: 1.2rem;
		margin: 20px 0;
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
		transform: scale(1.05);
	}

	/* Animations */
	@keyframes fadeIn {
		0% {
			opacity: 0;
		}
		100% {
			opacity: 1;
		}
	}

	@keyframes slideUp {
		0% {
			transform: translateY(30px);
			opacity: 0;
		}
		100% {
			transform: translateY(0);
			opacity: 1;
		}
	}

	@keyframes scaleUp {
		0% {
			transform: scale(0.8);
			opacity: 0;
		}
		100% {
			transform: scale(1);
			opacity: 1;
		}
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

	.fade-in {
		animation: fadeIn 1.5s ease-in-out;
	}

	.fade-in-delay {
		animation: fadeIn 2s ease-in-out;
	}

	.slide-up {
		animation: slideUp 1.5s ease-in-out;
	}

	.scale-up {
		animation: scaleUp 1.5s ease-in-out;
	}

	.bounce {
		animation: bounce 2s infinite;
	}

	/* About Section */
	.about {
		padding: 80px 20px;
		text-align: center;
	}

	.about p {
		max-width: 800px;
		margin: 20px auto;
		font-size: 1.1rem;
		line-height: 1.6;
	}

	/* Skills Section */
	.skills {
		background-color: #007acc;
		color: white;
		padding: 60px 20px;
		text-align: center;
	}

	.skills-grid {
		display: grid;
		grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
		gap: 20px;
		max-width: 800px;
		margin: 0 auto;
	}

	.skill-card {
		background-color: #00d1b2;
		padding: 20px;
		border-radius: 10px;
		animation: scaleUp 1.5s ease-in-out;
	}

	/* Projects Section */
	.projects {
		padding: 80px 20px;
		background-color: #f4f4f4;
		text-align: center;
	}

	.project-grid {
		display: grid;
		grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
		gap: 20px;
		max-width: 1000px;
		margin: 0 auto;
	}

	.project-card {
		background-color: white;
		padding: 20px;
		border-radius: 10px;
		box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
		transition: transform 0.3s ease;
		animation: scaleUp 1.5s ease-in-out;
	}

	.project-card:hover {
		transform: translateY(-10px);
	}

	/* Contact Section */
	.contact {
		padding: 80px 20px;
		background-color: #007acc;
		color: white;
		text-align: center;
	}

	.contact-btn {
		background-color: white;
		color: #007acc;
		padding: 15px 30px;
		font-size: 1.2rem;
		border-radius: 30px;
		margin-top: 20px;
		display: inline-block;
		animation: bounce 2s infinite;
		transition: background-color 0.3s ease;
	}

	.contact-btn:hover {
		background-color: #00d1b2;
		color: white;
	}
</style>
