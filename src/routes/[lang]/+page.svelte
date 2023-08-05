<script>
	import { i, languages, switchLanguage, language } from "@inlang/sdk-js"

	const title = 'Serenity Alang-Alang and Bamboo';
	const description =
		'We are a business leading in the construction of various bamboo structure, housing, and custom bamboo design made to order';
</script>


{#each languages as lang}
	<button on:click={() =>switchLanguage(lang)}>{lang}</button>
{/each}

<h1>{i("welcome")}</h1>
<p>{language}</p>

<svelte:head>
	<title>{title}</title>
	<meta name="description" content={description} />
</svelte:head>

<h1>{title}</h1>
<p>{description}</p>