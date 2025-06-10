<script lang="ts">
	import "@app/styles/styles.less"

	import {DefaultLayout} from "@widgets/layout/default/ui";

	let { children } = $props();
</script>

<DefaultLayout>
	<header class="site-header" slot="header">
		<nav>
			<a href="/">Home</a>
			<a href="/about">About</a>
			<a href="/contact">Contact</a>
		</nav>
	</header>

	{@render children()}

	<footer class="site-footer" slot="footer">
		<p>&copy; 2025 Sad. All rights reserved.</p>
	</footer>
</DefaultLayout>
