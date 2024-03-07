<script>
	import CardMusica from '$components/CardMusica.svelte';

	let dischi = [
		{
			artista: 'System of a Down',
			disco: 'Toxicity',
			durata: '44:25',
			anno: '2001',
			image: 'https://upload.wikimedia.org/wikipedia/en/6/64/SystemofaDownToxicityalbumcover.jpg'
		},
		{
			artista: 'Tiberio',
			disco: 'Sugar',
			durata: '24:04',
			anno: '2002',
			image: 'https://upload.wikimedia.org/wikipedia/en/6/64/SystemofaDownToxicityalbumcover.jpg'
		},
		{
			artista: 'Frank',
			disco: 'prova',
			durata: '33:04',
			anno: '2023',
			image: 'https://upload.wikimedia.org/wikipedia/en/6/64/SystemofaDownToxicityalbumcover.jpg'
		}
	];
</script>

<svelte:head>
	<link rel="stylesheet" href="https://unpkg.com/tailwindcss@3.4.1/src/css/preflight.css" />
</svelte:head>

{#each dischi as disco}
	<CardMusica
		artista={disco.artista}
		disco={disco.disco}
		durata={disco.durata}
		anno={disco.anno}
		image={disco.image}
	/>
{/each}
