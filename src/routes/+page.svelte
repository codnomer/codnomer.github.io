<script>
	import { Hero, Carousel, CarouselItem, Badge } from 'spaper';
</script>

<div class="container">
	<div class="content">
		<h3>
			<Badge type="primary">Hi</Badge>, My name is <Badge type="secondary">Omer Demirhan</Badge>
			I am a <Badge type="success">Full-Stack</Badge> Software Developer.
		</h3>
		<h4>
			I love learning new technologies because, as Steve Jobs famously said, 'Stay hungry, stay
			foolish,' meaning never lose the desire to learn and always stay curious
		</h4>

		<!-- <div class="gallery">
			<img src="jq.webp" alt="Two hands creating a heart and showing the sun" />
			<img src="starwars.webp" alt="The mountain" />
			<img src="pg.webp" alt="a river" />
			<img src="pg.webp" alt="a river" />
			<img src="pg.webp" alt="a river" /><img src="pg.webp" alt="a river" />
			<img src="https://picsum.photos/id/823/400/400" alt="a women with a camera" />
		</div> -->
		<h5>my tech stack</h5>
		<div class="gallery">
			<img src="jss.png" alt="a house on a mountain" />
		</div>
		<div class="gallery">
			<img src="node.png" alt="sime pink flowers" />
		</div>
		<div class="gallery">
			<img src="rust.png" alt="big rocks with some trees" />
		</div>

		<div class="gallery">
			<img src="svelte.png" alt="a cool landscape" />
		</div>
		<div class="gallery">
			<img src="jq.webp" alt="inside a town between two big buildings" />
		</div>
		<div class="gallery">
			<img src="pg.webp" alt="postgresql" />
		</div>
		<!-- <Carousel --min-height="100px" --max-height="300px">
			<CarouselItem>
				<img src="starwars.webp" />
			</CarouselItem>
			<CarouselItem>
				<img src="https://picsum.photos/id/22/600/300" />
			</CarouselItem>
			<CarouselItem>
				<img src="https://picsum.photos/id/25/600/300" />
			</CarouselItem>
			<CarouselItem>
				<img src="https://picsum.photos/id/43/600/300" />
			</CarouselItem>
			<CarouselItem>
				<img src="https://picsum.photos/id/45/600/300" />
			</CarouselItem>
		</Carousel> -->
	</div>
</div>

<style>
	.container {
		display: flex;
		justify-content: center;
		align-items: center; /* Optional: vertically center the content */
		/* Optional: adjust the height as needed */
	}

	.content {
		text-align: center; /* Optional: center the text within the div */
	}
	div.gallery {
		margin: 5px;

		float: left;
		width: 180px;
	}

	div.gallery img {
		width: 100%;
		object-fit: contain;
		height: 100px;
	}
</style>
