<script lang="ts">
	let { data } = $props();
</script>

<div class="main">
	<div class="top">
		<h1 class="title">{data.title}</h1>
	</div>
	<div class="middle">
		<p><strong>Location:</strong> {data.location}</p>
	</div>
	<p class="description">
		{data.description}
	</p>
</div>

<style>
	.main {
		display: flex;
		flex-direction: column;
		border: solid 1px black;
		border-radius: 10px;
		width: 20%;
		font-weight: normal;
	}
	.top {
		width: 100%;
		border-bottom: solid 1px black;
	}

	.title {
		font-size: 1.5rem;
		padding-left: 1rem;
	}
	.middle {
		border-bottom: solid 1px black;
		width: 100%;
	}

	.middle p {
		padding-left: 1rem;
	}

	.description {
		padding-left: 1rem;
		font-weight: normal;
	}
</style>
