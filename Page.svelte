<script>
  export let variant;
</script>

<style>
  @page {
    size: letter;
    margin: 0.5in;
  }

  @page :right {
    margin-top: 1in;

    @top-left {
      content: element(odd-header);
    }
  }

  #odd-header {
    position: running(odd-header);
    border: 1px solid black;
    padding: 0.1in;
  }
</style>

<div id="odd-header">
  Student Name
</div>

<ol>
  <slot />
</ol>