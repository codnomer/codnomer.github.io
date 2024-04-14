<!-- Your JavaScript and CSS -->
<script>
	import { Card, Button, Badge } from 'spaper';
</script>

<!-- Your HTML structure -->
<div class="container">
	<div class="card">
		<div class="card-body">
			<div class="image-container">
				<img src="actix.png" class="card-image" />
			</div>
			<h4 class="card-title">Backend’in Verstappen’i Actix-Web</h4>
			<div class="badge-container">
				<Badge type="warning" rounded>Rust</Badge>
				<Badge type="danger" rounded>Backend</Badge>
			</div>
			<div class="card-bottom">
				<p></p>
				<Button
					type="success"
					href="https://medium.com/@codnomer/backendin-verstappen-i-actix-web-e23bf6b0aea8"
					external>Read</Button
				>
			</div>
		</div>
	</div>
	<div class="card">
		<div class="card-body">
			<div class="image-container">
				<img src="webassembly.png" class="card-image" />
			</div>
			<h4 class="card-title">Frodo “Rust” Baggins — WebAssembly</h4>
			<div class="badge-container">
				<Badge type="warning" rounded>Rust</Badge>
				<Badge type="danger" rounded>WebAssembly</Badge>
			</div>
			<div class="card-bottom">
				<p></p>
				<Button
					type="success"
					href="https://medium.com/@codnomer/frodo-rust-baggins-webassembly-2d183f2eb371"
					external>Read</Button
				>
			</div>
		</div>
	</div>
	<div class="card">
		<div class="card-body">
			<div class="image-container">
				<img src="js.webp" class="card-image" />
			</div>
			<h4 class="card-title">JavaScript++ ( Web Assembly)</h4>
			<div class="badge-container">
				<Badge type="warning" rounded>Rust</Badge>
				<Badge type="danger" rounded>WebAssembly</Badge>
			</div>
			<div class="card-bottom">
				<p></p>
				<Button
					type="success"
					href="https://medium.com/@codnomer/javascript-web-assembly-d64f9d43d992"
					external>Read</Button
				>
			</div>
		</div>
	</div>
	<div class="card">
		<div class="card-body">
			<div class="image-container">
				<img src="marka.webp" class="card-image" />
			</div>
			<h4 class="card-title">Markasal Benlik</h4>
			<div class="badge-container">
				<Badge type="success" rounded>Random</Badge>
			</div>
			<div class="card-bottom">
				<p></p>
				<Button
					type="success"
					href="https://medium.com/@codnomer/markasal-benlik-acc00029d216"
					external>Read</Button
				>
			</div>
		</div>
	</div>
	<div class="card">
		<div class="card-body">
			<div class="image-container">
				<img src="is.webp" class="card-image" />
			</div>
			<h4 class="card-title">Kariyer Planlaması Yapan Veri — İş Zekası</h4>
			<div class="badge-container">
				<Badge type="success" rounded>Random</Badge>
			</div>
			<div class="card-bottom">
				<p></p>
				<Button
					type="success"
					href="https://medium.com/@codnomer/kariyer-planlamas%C4%B1-yapan-veri-i%CC%87%C5%9F-zekas%C4%B1-ad94fb123b22"
					external>Read</Button
				>
			</div>
		</div>
	</div>
	<div class="card">
		<div class="card-body">
			<div class="image-container">
				<img src="yagni.webp" class="card-image" />
			</div>
			<h4 class="card-title">Yazılım Prensibleri — YAGNI</h4>
			<div class="badge-container">
				<Badge type="success" rounded>Software</Badge>
			</div>
			<div class="card-bottom">
				<p></p>
				<Button
					type="success"
					href="https://medium.com/@codnomer/yaz%C4%B1l%C4%B1m-prensibleri-yagni-1eada215adc9"
					external>Read</Button
				>
			</div>
		</div>
	</div>
	<div class="card">
		<div class="card-body">
			<div class="image-container">
				<img src="arrayset.webp" class="card-image" />
			</div>
			<h4 class="card-title">JavaScript Anahtarlı Koleksiyonlar</h4>
			<div class="badge-container">
				<Badge type="success" rounded>JavaScript</Badge>
			</div>
			<div class="card-bottom">
				<p></p>
				<Button
					type="success"
					href="https://medium.com/@codnomer/javascript-anahtarl%C4%B1-koleksiyonlar-870de723c0e2"
					external>Read</Button
				>
			</div>
		</div>
	</div>
	<div class="card">
		<div class="card-body">
			<div class="image-container">
				<img src="jq.webp" class="card-image" />
			</div>
			<h4 class="card-title">yaşlıkurt.js == ‘jQuery’</h4>
			<div class="badge-container">
				<Badge type="success" rounded>JavaScript</Badge>
				<Badge type="warning" rounded>jQuery</Badge>
			</div>
			<div class="card-bottom">
				<p></p>
				<Button
					type="success"
					href="https://medium.com/@codnomer/ya%C5%9Fl%C4%B1kurt-js-jquery-840979c94739"
					external>Read</Button
				>
			</div>
		</div>
	</div>
	<div class="card">
		<div class="card-body">
			<div class="image-container">
				<img src="pg.webp" class="card-image" />
			</div>
			<h4 class="card-title">Cod name is Postgres</h4>
			<div class="badge-container">
				<Badge type="success" rounded>Postgres</Badge>
				<Badge type="danger" rounded>English</Badge>
			</div>
			<div class="card-bottom">
				<p></p>
				<Button
					type="success"
					href="https://medium.com/@codnomer/cod-name-is-postgres-377d879efb6"
					external>Read</Button
				>
			</div>
		</div>
	</div>
</div>

<style>
	.container {
		display: grid;
		grid-template-columns: repeat(
			auto-fill,
			minmax(300px, 1fr)
		); /* Create auto-fill columns with a minimum width of 300px */
		grid-gap: 20px; /* Add gap between cards */
		justify-items: center; /* Center cards horizontally */
	}
	.card {
		width: 250px; /* Adjust the width of the card */
		border: 1px solid #ccc;
		border-radius: 5px;
		margin: 5px;
	}

	.card-body {
		padding: 10px;
	}

	.image-container {
		height: 200px; /* Set a fixed height for the image container */
		overflow: hidden;
		display: flex;
		justify-content: center;
		align-items: center;
	}

	.card-image {
		max-width: 100%; /* Ensure the image does not exceed the container width */
		max-height: 100%; /* Ensure the image does not exceed the container height */
	}

	.card-title {
		font-size: 22px;
		margin-top: 10px;
	}

	.badge-container {
		margin-top: 10px;
	}

	.badge {
		margin-right: 5px;
	}

	.card-bottom {
		margin-top: 10px;
		text-align: center;
	}
</style>
