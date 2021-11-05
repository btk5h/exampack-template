<script>
  export let height = 1;
</script>

<style>
  .question {
    break-inside: avoid;
  }

  .response {
    border: 1px solid black;
    height: calc(0.5in * var(--height));
  }
</style>

<li class="question">
  <slot />

  <div class="response" style="--height: {height}" />
</li>