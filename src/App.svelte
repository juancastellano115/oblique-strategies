<script>
  import Strategy from "./components/Strategy.svelte";
</script>

<main>
  <Strategy />
</main>

<style>
  main {
    text-align: center;
    padding: 0px;
    margin: 0 0;
	display: flex;
	flex-direction: column;
	justify-content: center;
	align-items: center;
	height: 100%;
  }

  @media (min-width: 640px) {
    main {
      max-width: none;
    }
  }
</style>
