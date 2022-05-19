<script context="module">
	import { browser, dev } from '$app/env';

	// we don't need any JS on this page, though we'll load
	// it in dev so that we get hot module replacement...
	// export const hydrate = dev;

	// ...but if the client-side router is already loaded
	// (i.e. we came here from elsewhere in the app), use it
	// export const router = browser;

	// since there's no dynamic data here, we can prerender
	// it so that it gets served as a static asset in prod
	// export const prerender = true;


	import SvelteMarkdown from 'svelte-markdown'
	const source = `# Acknowledgements
### Outside libraries used:
  * **GUI:**              [Dear ImGui](https://github.com/ocornut/imgui) & [imgui_markdown](https://github.com/juliettef/imgui_markdown)
  * **Serialization:**    [Boost](https://www.boost.org/)
  * **OpenGL Rendering:** [GLEW](http://glew.sourceforge.net/) & [GLFW](https://www.glfw.org/)
  * **Math:**             [GLM](https://github.com/g-truc/glm)
  * **Image Loading:**    [stb_image](https://github.com/nothings/stb)

### Font:
[JetBrains Mono](https://www.jetbrains.com/lp/mono/)`

</script>

<svelte:head>
	<title>About</title>
</svelte:head>

<div class="content">
	<SvelteMarkdown {source} />
</div>

<style>
	.content {
		width: 100%;
		max-width: var(--column-width);
		margin: var(--column-margin-top) auto 0 auto;
	}
</style>
