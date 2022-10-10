<script>
	const newDevices = [
	{ 
		date: 'Oct 09', 
		title: 'CC Remap and Block',
		description: 'A simple yet very useful device to block or remap any Control Change midi message.'
	},
	{
		date: 'Oct 09',
		title: 'JChorus Juno-style BBD chorus',
		description: 'This specializes in conjuring lush stereo pads, but also works great on leads...'
	},
	{
		date: 'Oct 09',
		title: 'FocusEQ',
		description: 'This EQ "ranges" the three bands with the position of the Lowpass + Highpass filters.'
	},
	{ 
		date: 'Oct 06',
		title: 'Max Sticker',
		description: '文字便签小工具。插入轨道，可以简单记录些文字。 空格友好，不用担心再'
	},
	{
		date: 'Oct 06',
		title: 'Project Timer',
		description: '工程计时工具。插入工程轨道开始计时。 支持严格计时，当工程超过5分钟'
	}
	]
	const categories = [
		{ title: 'MIDI Devices', desc: 'Transform and manipulate MIDI information'},
		{ title: 'Audio Devices', desc: 'Effects, instruments and anything that processes audio'},
		{ title: 'Push', desc: 'Customise how you interact with the Ableton Push through M4L'},
		{ title: 'MIDI Instruments', desc: 'Generate MIDI data'},
    	{ title: 'LFO', desc: 'Bespoke oscillators for parameter control and modulation'},
		{ title: 'Sequencers', desc: 'Sequence MIDI information'},
		{ title: 'Drum Machine', desc: 'A variety of drum machines and rhythmic devices'},
		{ title: 'Sample Glitch', desc: 'Devices for glitching audio samples'},
		{ title: 'Effects', desc: 'Audio effects'},
		{ title: 'Jitter/Video', desc: 'Manipulate video through jitter'},
		{ title: 'Utility', desc: 'Various utility devices for making your life easier'},
		{ title: 'Experimental', desc: "Devices that don't necessarily fit into the other categories" }
	]
</script>

<div class="centre">
	<div class="categories">
		<h2>Device Categories</h2>
		<div class="cats">
			{#each categories as c}
			<div class="category">
				<div class="title">{ c.title }</div>
				<div class="desc">{ c.desc }</div>
			</div>
			{/each}
		</div>
	</div>
	<div class="new">
		<h2>Newest Devices</h2>
		{#each newDevices as device}
		<div class="device">
			
			<h3 class="title"> 
				{ device.title }
				<div class="date">{ device.date }</div>
			</h3>
			<div class="desc"> { device.description }</div>
		</div>
		{/each}
	</div>
</div>

<style>
	.centre {

	}

	.category {
		display: flex;
		flex-direction: column;
		width: 150px;
		background-color: #f0f0f0;
		padding: 1em;
	}

	.category > .title {
		font-weight: bold;
	}

	.category > .desc {
		font-size: 0.75rem;
	}

	.cats {
		display: flex;
		flex-direction: row;
		gap: 0.25em;
		flex-wrap: wrap;

	}

	h2 {
		border-bottom: 4px solid #f0f0f0
	}
	
	.new {
		display: flex;
		flex-direction: column;
		gap: 0.25em;
	}

	.device {
		background-color: #f0f0f0;
		padding: 1em;
		padding-top: 0.25em;
	}

	.category:hover, .device:hover {
		outline: 2px solid black;
		cursor: pointer;
	}

	.date {
		font-size: 0.75rem;
		color: #747474;
	}
	.desc {
		color: #747474;
	}
</style>