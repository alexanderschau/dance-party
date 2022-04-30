<script lang="ts">
  export let imageUrls: string[];
</script>

<div class="my-8 w-max">
  <div class="bg inline-block h-1/2">
    {#each imageUrls as image}
      <img
        alt="a nice party gif :("
        src={"https://media.giphy.com/media/" + image + "/giphy.gif"}
        loading="lazy"
        class="mx-4 inline-block h-full"
      />
    {/each}
  </div>
  <div class="bg inline-block h-1/2">
    {#each imageUrls as image}
      <img
        alt="a nice party gif :("
        src={"https://media.giphy.com/media/" + image + "/giphy.gif"}
        loading="lazy"
        class="mx-4 inline-block h-full"
      />
    {/each}
  </div>
</div>

<style>
  .bg {
    transform: translateY(0);
    animation: background-shift 20s linear infinite forwards;
  }
  @keyframes background-shift {
    to {
      transform: translateX(-100%);
    }
  }
</style>
