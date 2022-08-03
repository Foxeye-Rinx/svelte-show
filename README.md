# svelte-show

Like `v-show` in `vuejs`, or `ng-show` in `angularjs`, `svelte-show` just hide the element, it does not destroy the components inside its block.
This library is used for cases when we need to keep the HTML elements retain in DOM, to avoid re-initialization when working with some 3rd libraries.
## Usage

```svelte
<script>
  import Show from "svelte-show/Show.svelte";
  let show = true;
</script>
<button on:click={() => { show = !show}}>
  Click to Show/Hide Content
</button>
<Show {show}>
  <div>Content</div>
</Show>
```