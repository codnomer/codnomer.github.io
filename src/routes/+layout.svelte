<!-- src/routes/_layout.svelte -->
<script>
	// Import the CSS file globally
	import { Navbar, Button } from 'spaper';
	import 'papercss/dist/paper.min.css';
</script>

<div style="display: contents">
	<!-- This will render the content of each page -->
	<div class="container-md">
		<!-- Your bottom navbar content goes here -->
		<Navbar>
			<h3 slot="brand">
				<a href="/">codnomer</a>
			</h3>
			<ul class="inline">
				<li><a href="/blog">Blog</a></li>
				<li><a href="/about">About</a></li>
				<li><a href="/ideas">Ideas</a></li>
				<li>
					<Button>Project</Button>
				</li>
			</ul>
		</Navbar>
	</div>
	<slot />
</div>

<style>
</style>
