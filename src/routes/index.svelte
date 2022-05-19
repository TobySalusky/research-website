<script context="module">
	export const prerender = true;
</script>
<script>
	import ExampleCarousel from '../components/ExampleCarousel.svelte';
</script>

<svelte:head>
	<title>Home</title>
</svelte:head>

<section>
	<div class='content_scroll'>
		<h1 class='title'>
			MeshPencil
		</h1>
		<h3 class='subtitle'>
			A 2D Workflow for Organic 3D Modeling & Animation
		</h3>
		<div class="welcome">
			<ExampleCarousel/>
		</div>
	</div>
	
	<div class='description_body'>
		<div class='cool_box'>
			<h1><b>Instant Feedback 🔥</b></h1>
			<img src='images/info/Squid.gif' alt='creation of a squid model'>
			<h3>Create models in real time with user-drawn curves!</h3>
		</div>
		<div class='cool_box'>
			<h1><b>Animation Made Easy</b></h1>
<!--			<img src='images/info/Squid.gif' alt='creation of a squid model'>-->
			<h3>Avoid bone-based rigging by treating curves themselves like key-frames!</h3>
		</div>
		
		<div class='download_now'>
			<h1>Download</h1>
		</div>
	</div>
</section>

<style>
	.description_body {
		margin-top: 3vh;
		width: 80vw;
		margin-bottom: 500vh;
		
		display: flex;
		flex-direction: column;
		align-items: center;
	}
	
	.download_now, .cool_box, .cool_box img {
		box-shadow: rgba(0, 0, 0, 0.07) 0px 1px 1px, rgba(0, 0, 0, 0.07) 0px 2px 2px, rgba(0, 0, 0, 0.07) 0px 4px 4px, rgba(0, 0, 0, 0.07) 0px 8px 8px, rgba(0, 0, 0, 0.07) 0px 16px 16px;	}
	
	.download_now {
		margin-top: 5vh;
		background-color: var(--program-background-color);
		padding-block: 2em;
		padding-inline: 10em;
	}
	
	.download_now h1 {
		color: white;
	}
	
	.cool_box {
		background-color: #c1c1c1;
		display: flex;
		justify-content: center;
		align-items: center;
		padding-block: 1vh;
		padding-inline: 2vw;
		flex-direction: column;
		width: fit-content;
		
		margin-block: 2vh;
	}
	
	.cool_box img {
		width: 40vw;
		border-radius: 3px;
	}
	
	.cool_box h1, .cool_box h3 {
		color: var(--header-border-color)
	}
	
	.title {
		color: white;
		font-size: 4em;
		padding: 1rem 0 0;
		margin: 0;
	}
	.subtitle {
		color: gray;
		font-size: 1.2em;
		padding: 0;
		margin: 0;
		text-align: center;
		font-weight: normal;
	}
	
	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 1;
	}

	h1 {
		width: 100%;
	}
	
	.content_scroll {
		width: 100vw;
		background-color: var(--program-background-color);
	}
	
	.welcome {
	}
</style>
