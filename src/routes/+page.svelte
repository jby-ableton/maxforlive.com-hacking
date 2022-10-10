<script>
	import Header from '$lib/components/Header.svelte';
	import Account from '$lib/components/Account.svelte';
	import Centre from '$lib/components/Main/Centre.svelte';
	import Sidebar from '$lib/components/Main/Sidebar.svelte';
</script>

<Header />
<Account />

<main>
	<Centre />
	<Sidebar />
</main>

<style>
	main {
		display: grid;
		grid-template-columns: auto auto;
	}
</style>