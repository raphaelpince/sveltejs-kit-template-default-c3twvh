<script>
	import Header from './Header.svelte';
	import './styles.css';
</script>

<div class="app">
	<Header />

	<main>
		<slot />
	</main>



</div>
<footer>
<br>
<br>
<br>
<a href="https://www.instagram.com/raphael.pnc/?hl=fr">
  <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/a/a5/Instagram_icon.png/640px-Instagram_icon.png" alt="Mon instagram"
	width="30"
	height="30">
</a>

<a href="https://twitter.com/RaphaelPince">
  <img src="https://i.notretemps.com/1800x0/smart/2017/06/06/logo-twitter.jpg" alt="Mon Twitter"
	width="40"
	height="30">
</a>

<a href="https://www.leagueofgraphs.com/fr/summoner/euw/r6lasaucisse">
  <img src="https://logo-marque.com/wp-content/uploads/2020/11/League-of-Legends-Embleme.png" alt="Mon Twitter"
	width="50"
	height="30">
</a>

</footer>
<style>
a {
	float:right;
}
	.app {
		display: flex;
		flex-direction: column;
		min-height: 100vh;
	}

	main {
		flex: 1;
		display: flex;
		flex-direction: column;
		padding: 1rem;
		width: 100%;
		max-width: 64rem;
		margin: 0 auto;
		box-sizing: border-box;
	}



</style>
