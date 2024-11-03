<script>
  import { page } from "$app/stores";
  console.log();

  const slugArr = $page.params.slug.split("/");
</script>

<h1>Docs homepage</h1>
{#if slugArr.length === 1}
  <h1>Viewing docs for feature {slugArr[0]}</h1>
{:else if slugArr.length === 2}
  <h1>Viewing docs for sub-feature {slugArr[0]} - {slugArr[1]}</h1>
{/if}
