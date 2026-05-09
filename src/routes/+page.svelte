<script>
  import words from '$lib/data/words.json'
  import { onMount } from 'svelte'

  let selectedWord = $state(words[0])

  function pickRandom() {
    selectedWord = words[Math.floor(Math.random() * 450)]
  }

  onMount(pickRandom)

</script>

<div class="stack box" style="max-inline-size: 500px">
  <article class="card">
    <figure>
      <img
        src="https://image.pollinations.ai/prompt/{selectedWord.en}"
        width=622 height=350
        alt="Image_Not_Found"
      />
    </figure>
    <header>
      <h4>{selectedWord.es}</h4>
      <span class="tag muted">{selectedWord.type}</span>
    </header>
    <div class="card-body stack">
      <p>{selectedWord.pronunciation}</p>
    </div>
    <footer class="cluster">
      <button onclick={pickRandom}>Next</button>
    </footer>
  </article>

</div>


<style>


</style>