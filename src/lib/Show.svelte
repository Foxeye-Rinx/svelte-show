<script>
  export let show = true;
</script>

<div class:hide={!show}>
  <slot />
</div>

<style>
  .hide {
    visibility: hidden !important;
    height: 0 !important;
    padding: 0 !important;
    margin: 0 !important;
  }
</style>
