<header>
	<div class="left">
		<input />
		<button>Search</button>
	</div>

	<div class="right">
		<a href="/">Home</a>
		<a href="/">Login</a>
		<a href="/">Help</a>
		<a href="/">Contact</a>
		<a href="/">RSS</a>
	</div>
</header>


<style>
	header {
		height: 33.6px;
		background-color: black;
		display: flex;
		justify-content: space-between;
		margin-bottom: 0.25rem;
		align-items: center;
		padding-left: 1em;
		padding-right: 1em;
	}

	input {
		background-color: #bbbbbb;
		border: none;
		font-family: Verdana, Geneva, Tahoma, sans-serif;
	}

	button {
		font-family: Verdana, Geneva, Tahoma, sans-serif;
	}

	.right {
		display: flex;
		flex-direction: row;
		gap: 1em;;
	}

	a {
		color: #cccccc;
	}
	a:hover {
		color: #0293b4;
	}
</style>