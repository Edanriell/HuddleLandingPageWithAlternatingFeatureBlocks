<script lang="ts">
	import {goto} from "$app/navigation";

	import {Button} from "@shared/ui/button/ui";

	function goHome() {
		goto('/');
	}

	function goBack() {
		history.back();
	}
</script>

<svelte:head>
	<title>Page Not Found - 404</title>
	<meta content="The page you're looking for could not be found." name="description" />
</svelte:head>

<div class="min-h-screen flex items-center justify-center bg-gray-50 px-[16rem]">
	<div class="w-full max-w-[1024rem] text-center">
		<div class="mb-[48rem]! mt-[48rem]">
			<h1 class="mb-[unset]! mt-[unset]! text-[128rem]! sm:text-[144rem]! desktop:text-[192rem]! font-bold! text-gray-200! select-none!">404</h1>
		</div>
		<div class="mb-[48rem] max-w-[512rem] mx-auto">
			<h2 class="text-[48rem]! sm:text-[64rem]! desktop:text-[60rem]! font-bold! text-gray-900! mb-[24rem]!">Page Not Found</h2>
			<p class="text-[16rem]! desktop:text-[18rem]! text-gray-600! mb-[32rem]! leading-[150%]!">
				Sorry, we couldn't find the page you're looking for.
				It might have been moved, deleted, or you entered the wrong URL.
			</p>
		</div>
		<div class="flex flex-col sm:flex-row gap-[16rem] justify-center mb-[64rem]">
			<Button className="max-w-[280rem]! ml-auto! mr-auto!" colorScheme="Pink" onclick={goHome}>
				Go Home
			</Button>
			<Button className="max-w-[280rem]! ml-auto! mr-auto!" colorScheme="Pink" onclick={goBack}>
				Go Back
			</Button>
		</div>
	</div>
</div>

<style>
	@keyframes float {
		0%, 100% { transform: translateY(0rem); }
		50% { transform: translateY(-10rem); }
	}

	h1 {
		animation: float 3s ease-in-out infinite;
	}
</style>