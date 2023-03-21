<!--This is a wrapper around all other content on your website. Things here
should be on every page, such as a header, footer, or the loading of global
styles.-->
<!--Also required by Tailwind CSS to load in the global Tailwind Styles.-->
<script>
  import "../app.css";
	import Footer from '$lib/components/Footer.svelte';
	import Header from '$lib/components/Header.svelte';
</script>

<Header />

<!--This is the main content on every page-->
<slot />

<Footer />
