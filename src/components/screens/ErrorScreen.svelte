<script>
	export let message;
	export let status;
</script>


<div class='content'>
	<h1 class='error'>Error ({status})</h1>
	<h2>{message}</h2>
	<div class='image_block'>
		<h3 class='commentary'>Uh oh.</h3>
		<img src='images/ErrorShock.gif' alt='porpoise-like creature shocked by error'>
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
		margin-bottom: 0;
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
		padding-bottom: 2em;
	}
	.commentary {
		color: #999999;
		text-align: center;
	}
	h2 {
		color: indianred;
		text-align: center;
	}
</style>