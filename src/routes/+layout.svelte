<!-- src/routes/_layout.svelte -->
<script>
	// Import the CSS file globally
	import { Navbar, Button } from 'spaper';
	import 'papercss/dist/paper.min.css';
	let navLinks = [
		{ name: 'About', link: '/about' },
		{ name: 'Blog', link: '/blog' },
		{ name: 'Ideas', link: '/ideas' }
	];

	let contactLink = 'mailto:demirhanomer11@gmail.com';
	let isMenuOpen = false;

	// Function to toggle mobile menu
	function toggleMenu() {
		isMenuOpen = !isMenuOpen;
	}
</script>

<div style="display: contents">
	<!-- This will render the content of each page -->
	<div class="container-md">
		<!-- Your bottom navbar content goes here -->
		<Navbar>
			<h3 slot="brand">
				<a href="/">codnomer</a>
			</h3>
			<ul class="inline {isMenuOpen ? 'active' : ''}">
				{#each navLinks as navLink}
					<li>
						<a href={navLink.link}>{navLink.name}</a>
					</li>
				{/each}
				<li>
					<Button href={contactLink} class="contact-btn">Contact</Button>
				</li>
			</ul>
		</Navbar>
	</div>
	<slot />
</div>

<style>
</style>
