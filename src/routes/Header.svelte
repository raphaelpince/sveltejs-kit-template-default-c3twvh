<script>
	import { page } from '$app/stores';

</script>
<header>
<h1> Raphaël PINCE <h1>
	<nav>
	
		<ul>
			<li class:active={$page.url.pathname === '/'}>
				<a href="/">Home</a>
			</li>
			<li class:active={$page.url.pathname === '/bio'}>
				<a href="/bio">bio</a>
			</li>
			<li class:active={$page.url.pathname.startsWith('/myquiver')}>
				<a href="/myquiver">My quiver</a>
			</li>
			<li class:active={$page.url.pathname === '/Contact'}>
				<a href="/Contact">contact</a>
			</li>
		</ul>
		
	</nav>

</header>



<style>


	h1 {
		display : center;
		font-size: 20px;
    text-align: center;
		

	}


	header {
		display : center;
		justify-content: space-between;
		border-left : solid;
		border-left-color :  grey ;
		border-right : solid;
		border-right-color :  grey ;
		border-top : solid;
		border-top-color :  grey ;
	}


	nav {
		display: flex;
		justify-content: center;
		
	}



	ul {
		position: relative;
		padding: 0;
		margin: 0;
		height: 3em;
		display: flex;
		justify-content: center;
		align-items: center;
		list-style: none;
		background: var(--background);
		background-size: contain;
		font-size: 10px;
		border-left : solid;
		border-left-color :  grey ;
		border-right : solid;
		border-right-color :  grey ;
	}

	li {
		position: relative;
		height: 100%;
		
	}

	li.active::before {
		--size: 6px;
		content: '';
		width: 0;
		height: 0;
		position: absolute;
		top: 0;
		left: calc(50% - var(--size));
		border: var(--size) solid transparent;
		border-top: var(--size) solid var(--color-theme-1);
		
	}

	nav a {
		display: flex;
		height: 100%;
		align-items: center;
		padding: 0 0.5rem;
		color: var(--color-text);
		font-weight: 700;
		font-size: 0.8rem;
		text-transform: uppercase;
		letter-spacing: 0.1em;
		text-decoration: none;
		transition: color 0.2s linear;
		
	}

	a:hover {
		color: var(--color-theme-1);
		
	}

</style>
