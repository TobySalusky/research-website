<div class='content'>
	<h1 class='error'>404 Not Found</h1>
	<div class='image_block'>
		<h3 class='commentary'>This isn't where you're supposed to be...</h3>
		<img src='images/NotFound.png' alt='not found'>
		<h1 class='go_home'>
			> <a href='/'>Go Home?</a>
		</h1>
	</div>
</div>

<style>
	.content {
		display: flex;
		align-items: center;
		flex-direction: column;
	}
	.error {
		font-size: 5em;
	}
	.image_block {
		padding-inline: 5em;
		width: min-content;
		background-color: var(--program-background-color);
		display: flex;
		flex-direction: column;
		justify-content: center;
	}
	
	img {
		height: 20em;
		object-fit: contain;
	}
	.commentary {
		color: #999999;
		text-align: center;
	}
	.go_home {
		color: lightgray;
	}
	
	.go_home a {
		color: white;
	}
</style>