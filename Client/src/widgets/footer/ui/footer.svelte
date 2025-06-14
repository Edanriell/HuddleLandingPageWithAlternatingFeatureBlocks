<script lang="ts">
	import {Logotype} from "@shared/ui/logotype/ui";
	import {Contacts} from "@shared/ui/contacts/ui";
	import {SecondaryNavigation} from "@shared/ui/secondary-navigation/ui";
	import {SocialLinks} from "@shared/ui/social-link/ui";
	import {Copyright} from "@shared/ui/copyright/ui";
</script>

<footer class="pr-[16rem] pl-[16rem] pt-[139rem] pb-[46rem] bg-[#00252e] desktop:pr-[78rem] desktop:pl-[120rem] desktop:pt-[144rem] desktop:pb-[64rem] desktop:flex desktop:flex-row desktop:items-center desktop:justify-between">
	<div class="desktop:shrink-0 desktop:basis-[379rem] desktop:mr-[130rem]">
		<Logotype colorScheme="Light"/>
		<Contacts />
	</div>
	<div class="desktop:shrink-0">
		<SecondaryNavigation />
	</div>
	<div class="desktop:ml-[175rem] desktop:shrink-0 desktop:basis-[269rem] desktop:self-end desktop:flex desktop:flex-col desktop:items-start">
		<SocialLinks />
		<Copyright />
	</div>
</footer>