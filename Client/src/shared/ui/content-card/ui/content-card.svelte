<script lang="ts">
	let { title = "", description = "", className = "", contentClassName="", children } = $props();
</script>

<article class="rounded-[16rem] bg-white shadow-[0_0_14px_0_rgba(0,0,0,0.07)] min-h-[488rem] pt-[24rem]! pl-[40rem]! pr-[40rem]! pb-[33rem]! flex flex-col items-center justify-center desktop:flex-row desktop:justify-between desktop:pt-[unset]! desktop:pb-[unset]! desktop:pl-[120rem]! desktop:pr-[30rem]! desktop:min-h-[440rem] desktop:max-w-[1232rem] {className}">
	{@render children()}
	<div class="desktop:flex desktop:flex-col desktop:items-start {contentClassName}">
		<h3 class="mt-[24rem]! font-[var(--second-family)]! font-semibold! text-[20rem]! leading-[150%]! text-[#00252e]! text-center desktop:text-left desktop:mt-[unset]! desktop:text-[28rem]!">{title}</h3>
		<p class="mt-[16rem]! font-[var(--font-family)]! font-normal! text-[14rem]! leading-[150%]! text-center text-[#808e9a]! desktop:text-[18rem]! desktop:text-left">{description}</p>
	</div>
</article>