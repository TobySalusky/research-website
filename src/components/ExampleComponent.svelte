<script>
	export let name;
	export let type;
</script>

<div class='container'>
	<div class='img_container_1'>
		<img src='images/examples/{name}Top.{type}' alt='{name}'>
	</div>
	<div class='img_container_2'>
		<img src='images/examples/{name}Bottom.{type}' alt='{name}'>
	</div>
</div>

<style>
	.container {
		display: flex;
		align-items: center;
		flex-direction: column;
		width: 20vw;
		height: 30vw;
		padding-block: 3em;
	}
	
	.img_container_1, .img_container_2 {
		height: 50%;
		display: flex;
		align-items: center;
		justify-content: center;
	}
	
	.img_container_1 {
		width: 100%;
	}
	.img_container_2 {
		width: calc(100% - 1vw);
		padding-inline: 0.5vw;
	}
	
	img {
		max-width: 100%;
		max-height: 100%;
		object-fit: contain;
	}
</style>