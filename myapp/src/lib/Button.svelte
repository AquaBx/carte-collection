<script lang="ts">
	export let href : string | undefined = undefined
	export let icon : any = undefined

</script>


<a on:click href={href} class="flex justify-center gap-4 align-middle font-medium text-xl shadow-black/5 ring-1 ring-slate-700/10 appearance-none rounded-md w-full p-2 bg-slate-100 leading-none focus:outline hover:bg-slate-100/50 transition">
	<slot></slot>
	{#if icon}
		<svelte:component this={icon} weight="fill"/>
	{/if}
</a>