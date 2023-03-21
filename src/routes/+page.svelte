<script>
  import ExampleButton from '$lib/components/examples/ExampleButton.svelte';
	import profilePic from '$lib/assets/profile-pic.jpg';
</script>

<h1>This is your Landing Page To Your Portfolio Template</h1>
<h2>This is your main landing page</h2>


<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>

<p>Take a look at me!</p>
<img src='{profilePic}'
		 alt='profile pic'>

<p>This is an example of an imported button</p>
<ExampleButton>Click me</ExampleButton>

<!--All Style is Local To The Page/Component-->
<style>
	h1 {
		color: red;
	}

	h2 {
		color: green;
	}

	p {
		color: blue;
	}
</style>
