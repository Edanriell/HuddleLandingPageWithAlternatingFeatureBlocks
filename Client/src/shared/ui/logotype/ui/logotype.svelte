<script lang="ts">
	let { colorScheme } = $props();
</script>

{#if colorScheme === "Dark"}
	<a href="/" class="relative">
		<img class="w-[104rem] h-[16rem] desktop:w-[200rem] desktop:w-[31rem] object-contain" alt="Huddle company logotype" src="/images/raster/logotype_dark.png">
	</a>
{:else}
	<a href="/" class="relative">
		<img class="w-[167rem] h-[26rem] desktop:w-[152rem] desktop:w-[24rem] object-contain" alt="Huddle company logotype" src="/images/raster/logotype_light.png">
	</a>
{/if}