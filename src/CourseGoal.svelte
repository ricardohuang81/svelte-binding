<!-- scripts -->
<script>
  export let courseGoal;
  $: turnsRed = courseGoal.includes("!");
</script>

<!-- styles -->
<style>
  .turn-red {
    color: red;
  }
</style>

<!-- markup -->
<h1 class:turn-red="{turnsRed}">{courseGoal}</h1>