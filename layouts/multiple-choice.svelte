<script context="module">
  import OrderedList from "/components/OrderedList.svelte"; 
  export { 
    OrderedList as ul
  };
</script>

<style>
  .question {
    break-inside: avoid;
  }

  .question > :global(ol) {
    list-style: upper-alpha;
  }
</style>

<li class="question">
  <slot />
</li>