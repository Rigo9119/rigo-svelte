<script>
	import IndexButton from '../components/indexButton.svelte';
</script>

<section class="buttons">
	<IndexButton text="About" href="/about"/>
	<IndexButton text="Experience" href="/experience"/>
	<IndexButton text="Education" href="/education"/>
	<IndexButton text="Contact" href="/contact"/>
</section>

<style lang="scss">
	.buttons {
		align-items: center;
		display: flex;
		flex-flow: row wrap;
		height: 100vh;
		justify-content: space-between;
        margin: 40px 80px;
	}
</style>
