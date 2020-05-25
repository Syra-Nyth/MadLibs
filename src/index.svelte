<script>
	let output = ''
	let exclamation = ''
	let adverb = ''
	let noun = ''
	let adjective = ''
	
	function button() {
		output = `${exclamation} he said ${adverb} as he jumped into his convertible ${noun} and drove off with his ${adjective} wife.`
	}
</script>

<h1>MadLibs - Demo</h1>

<label>
  Exclamation (e.g. ouch):
  <input id="txtExcl" type="text" bind:value={exclamation}>
</label>
<br>
<label>
  Adverb (e.g. loudly):
  <input id="txtAdv" type="text" bind:value={adverb}>
</label>
<br>
<label>
  Noun (e.g. car):
  <input id="txtNoun" type="text" bind:value={noun}>
</label>
<br>
<label>
  Adjective (e.g. lovely):
  <input id="txtAdj" type="text" bind:value={adjective}>
</label>
<br>
<button on:click={button}>MadLib</button>

<p>
	{output}
</p>