<script>
  import words from '$lib/data/words.json'
  import { onMount } from 'svelte'

  let selectedWord = $state(words[0])

  function pickRandom() {
    selectedWord = words[Math.floor(Math.random() * 1000)]
  }

  onMount(pickRandom)

</script>

<h1>Welcome to Flash Espanol</h1>
<button onclick={pickRandom}>Next</button>
<h3>{selectedWord.es}</h3>
<img src="https://image.pollinations.ai/prompt/{selectedWord.en}" alt="{selectedWord.es}">

<style>
  * {
    padding: 1rem;
  }
</style>