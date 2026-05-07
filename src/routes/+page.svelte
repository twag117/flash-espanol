<script>
  import Words from '$lib/data/words.json'

  let words = Words
  let randomNumber = Math.floor(Math.random() * 1000) + 1
  let firstWord = words[randomNumber]
  console.log(firstWord)

</script>

<h1>Welcome to Flash Espanol</h1>
<p>{firstWord.es}</p>


<style>
  * {
    padding: 1rem;
  }
</style>