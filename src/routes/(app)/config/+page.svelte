<script lang="ts">
	//ParaglideJS
	import * as m from '@src/paraglide/messages';

	import PageTitle from '@src/components/PageTitle.svelte';
</script>

<div class="mb-2 flex items-center">
	<PageTitle name={m.config_pagetitle()} icon="" />
</div>

<h2 class="ml-2 mt-8 text-center text-tertiary-600 dark:text-primary-500">{m.config_body()}</h2>
<div class="mt-4 grid gap-4 sm:grid-cols-2 md:grid-cols-3">
	<!-- Collection -->
	<a href="/collection" class="variant-outline-tertiary btn gap-2 py-6 dark:variant-outline-secondary">
		<iconify-icon icon="mingcute:menu-fill" width="24" class="text-tertiary-600" />
		<p class="uppercase">{m.config_systembuilder()}</p>
	</a>

	<!-- builder to be replaced -->
	<a href="/builder" rel="external" class="variant-outline-tertiary btn gap-2 py-6 dark:variant-outline-secondary">
		<iconify-icon icon="fluent-mdl2:build-definition" width="24" class="text-error-600" />
		<p class="uppercase">{m.config_collectionbuilder()}</p>
	</a>

	<!-- Graphql Api -->
	<a href="/api/graphql" rel="external" class="variant-outline-tertiary btn gap-2 py-6 dark:variant-outline-secondary">
		<iconify-icon icon="teenyicons:graphql-solid" width="24" class="text-warning-600" />
		<p class="uppercase">{m.config_graphql()}</p>
	</a>

	<!-- Editor -->
	<a href="/imageEditor" class="variant-outline-tertiary btn gap-2 py-6 dark:variant-outline-secondary">
		<iconify-icon icon="bi:images" width="24" class="text-error-600" />
		<p class="uppercase">{m.config_imageeditor()}</p>
	</a>

	<!-- Dashboard -->
	<a href="/dashboard" class="variant-outline-tertiary btn gap-2 py-6 dark:variant-outline-secondary">
		<iconify-icon icon="bi:images" width="24" class="text-error-600" />
		<p class="uppercase">Dashboard</p>
	</a>
</div>
