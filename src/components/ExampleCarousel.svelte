<script>
	import { onMount } from 'svelte';
	import ExampleComponent from './ExampleComponent.svelte';
	
	let Carousel; // for saving Carousel component class
	let carousel; // for calling methods of the carousel instance
	onMount(async () => {
		const module = await import('svelte-carousel');
		Carousel = module.default;
	});
</script>


<svelte:component
	this={Carousel}
	bind:this={carousel}
	dots={false}
	arrows={false}
	autoplay={true}
	swiping={false}
	autoplayDuration={2000}
	particlesToShow={4}
>
	<ExampleComponent name='TeapotWave' type='gif'/>
	<ExampleComponent name='Ant' type='png'/>
	<ExampleComponent name='JakeRun' type='gif'/>
	<ExampleComponent name='Gary' type='png'/>
	<ExampleComponent name='Unwrap' type='gif'/>
	<ExampleComponent name='Mimikyu' type='png'/>
	<ExampleComponent name='CrabBounce' type='gif'/>
	<ExampleComponent name='Clover' type='png'/>
</svelte:component>

