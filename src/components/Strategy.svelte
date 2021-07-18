<script>
  import { strategies } from "../oblique";
  import Button, { Label, Icon } from "@smui/button";
  import sample from "lodash.sample";
  let phrase = "";

  function getStrategy() {
    phrase = sample(strategies);
  }

  getStrategy();
</script>

<div class="container">
  <h1>{phrase.strategy}</h1>

  <Button variant="raised" color="primary" on:click={getStrategy}>
    <Label>Another</Label>
    <Icon class="material-icons">replay</Icon>
  </Button>
</div>

<style>
  .container {
    padding: 1em;
  }
  h1 {
    color: white;
    font-size: 4em;
  }
  @media (max-width: 640px) {
    h1 {
      font-size: 2.4em;
    }
  }
</style>
