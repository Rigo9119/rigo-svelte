<script>
	export let href, text;
</script>

<a class="index-button" {href}>
	{text}
</a>

<style lang="scss">
	.index-button {
		align-items: center;
		border: 1px solid white;
		border-radius: 3px;
		background: black;
		color: rgb(163, 162, 162);
		display: flex;
		font-size: 3vmin;
		height: 225px;
		justify-content: center;
		letter-spacing: 18px;
		line-height: 20px;
		margin-bottom: 25px;
		padding: 15px;
		text-decoration: none;
		text-transform: uppercase;
		width: 48%;

		&:hover {
			color:rgb(221, 221, 221);
			background-color: crimson;
			border: 1px solid crimson;
			font-size: 5vmin;
		}
	}
</style>
