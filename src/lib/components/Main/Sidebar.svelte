<script>
	const updatedDevices = [
		'Spektral',
		'Source',
		'Scopium',
		'Bend Offset',
		'Max Sticker',
		'Linearscope',
		'WaveScope',
		'Get Trax',
		'Drumrack Toggle by Ableton',
		'Histoscope',
		'Fretboard',
		'Panner',
		'LASSTools-LA Scoring',
		'Iris Devices Mesh Visualisation',
		'Micron Industrialiser'
	]
</script>

<div class='container'>
	<div class="area">
		<h4 class="">Updated Devices</h4>
		<ul>
			{#each updatedDevices as ud}
			<li class='ud'>
				<a href="">{ ud }</a>
			</li>
			{/each}
		</ul>
	</div>

	<div class="area">
		<h4 class="">Resources</h4>
		<ul>
			<li class='ud'>
				<a href="">Max for Live Production Guidelines</a>
			</li>
		</ul>
	</div>

	<div class="area">
		<h4 class="">Library Stats</h4>
		<ul>
			<li class='ud'>
				<a href="">666 registered users</a>
			</li>
			<li>
				<a href="">74 shared devices</a>
			</li>
		</ul>
	</div>
</div>

<style>
	.container {
		background-color: #e6e7e7;
		margin: 0.25em;
		padding: 0.5em;
		font-size: 0.75rem;
		display: flex;
		flex-direction: column;
		justify-content: flex-start;
	}

	h4 {
		margin: 0;
	}

	ul {
		padding: 1em;
		margin: 0;
	}
	.ud {
		color: var(--blue);
		list-style-type: square;
	}
	li > a:visited {
		color: var(--blue);
	}
</style>