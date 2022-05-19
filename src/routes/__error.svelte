<!--suppress EqualityComparisonWithCoercionJS -->
<script context="module">
	export function load({ error, status }) {
		return {
			props: {
				message: error.message,
				status // same as status: status
			}
		};
	}
</script>

<script>
	import ErrorScreen from '../components/screens/ErrorScreen.svelte';
	import NotFoundScreen from '../components/screens/NotFoundScreen.svelte';

	export let message;
	export let status;
</script>

{#if status == 404} <!-- Used '==' to match string/number status code -->
	<NotFoundScreen />
{:else}
	<ErrorScreen {message} {status} />
{/if}
