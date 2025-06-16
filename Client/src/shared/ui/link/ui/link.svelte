<script lang="ts">
	let { colorScheme, href = "/", children } = $props();
</script>

{#if colorScheme === "White"}
	<a href={href} class="w-auto h-auto inline max-h-[24rem] rounded-[12rem] bg-white shadow-light-small font-[var(--font-family)] font-bold text-[10rem] text-[#00252e] pt-[6rem] pr-[22rem] pb-[4rem] pl-[23rem] desktop:max-h-[48rem] desktop:rounded-[24rem] desktop:shadow-light-large desktop:text-[14rem] desktop:pt-[13rem] desktop:pr-[63rem] desktop:pb-[16rem] desktop:pl-[65rem] hover:text-[#808e9a]">
		{@render children()}
	</a>
{:else}
	<a href={href} class="w-auto h-auto inline max-h-[40rem] rounded-[20rem] shadow-dark-small bg-[#ff52c1] font-[var(--font-family)] font-bold text-[12rem] text-white pt-[10rem] pr-[59rem] pb-[14rem] pl-[60rem] desktop:max-h-[56rem] desktop:rounded-[28rem] desktop:text-[14rem] desktop:pt-[17rem] desktop:pr-[69rem] desktop:pb-[20rem] desktop:pl-[70rem] hover:bg-[#ff9adb]">
		{@render children()}
	</a>
{/if}