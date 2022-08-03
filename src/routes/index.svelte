<script>
  import Show from "$lib/Show.svelte";
  let show = true;
</script>
<button on:click={() => { show = !show}}>
  Click to Show/Hide Content
</button>
<Show {show}>
  <div>Content</div>
</Show>