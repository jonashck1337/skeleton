<script>
	import Navbar from '../components/navbar.svelte';
	import photo1 from '../components/photo1.jpg';
	import photo2 from '../components/photo2.jpg';
	import photo3 from '../components/photo3.jpg';
	import photo4 from '../components/photo4.jpg';
    import linkedin from '../components/linkedin.png';
	import Map from '@anoram/leaflet-svelte';
	let options = {
		center: [48.83407644724074, 2.3716775921220727],
		markers: [
			{
				lat: 48.83407644724074,
				lng: 2.3716775921220727
			},
			{
				lat: 48.83407644724074,
				lng: 2.3716775921220727,
				popup: {
					isOpen: true,
					text: `Healthspace @ Station F`
				}
			}
		],
		mapID: 'map'
	};
</script>

<svelte:head>
	<title>About</title>
</svelte:head>

<Navbar />

<main>
	<div class="flex items-center justify-center h-32">
		<h1 class="text-2xl">Who are we?</h1>
	</div>

	<ul class="flex justify-center space-x-12">
		<li>
			<a href="#">
				<img class="h-48 w-48 rounded-full" src={photo3} alt="Antoine" />
			</a>
            <a class="flex flex-col items-center py-3 font-semibold text-lg text-blue-500">Antoine Chauvin</a>
            <a class="flex flex-col items-center py-1" href="https://www.linkedin.com/in/jonashecke/">
				<img class="h-5 w-5" src={linkedin} alt="linkedin_icon" />
			</a>
		</li>
        <li>
			<a href="#">
				<img class="h-48 w-48 rounded-full" src={photo4} alt="Inès" />
			</a>
            <a class="flex flex-col items-center py-3 font-semibold text-lg text-blue-500">Inès Mebarki</a>
            <a class="flex flex-col items-center py-1" href="https://www.linkedin.com/in/jonashecke/">
				<img class="h-5 w-5" src={linkedin} alt="linkedin_icon" />
			</a>
		</li>
        <li>
			<a href="#">
				<img class="h-48 w-48 rounded-full" src={photo2} alt="Raghav" />
			</a>
            <a class="flex flex-col items-center py-3 font-semibold text-lg text-blue-500">Raghav Bansal</a>
            <a class="flex flex-col items-center py-1" href="https://www.linkedin.com/in/jonashecke/">
				<img class="h-5 w-5" src={linkedin} alt="linkedin_icon" />
			</a>
		</li>
        <li>
			<a href="#">
				<img class="h-48 w-48 rounded-full" src={photo1} alt="Jonas" />
			</a>
            <a class="flex flex-col items-center py-3 font-semibold text-lg text-blue-500">Jonas Hecke</a>
            <a class="flex flex-col items-center py-1" href="https://www.linkedin.com/in/jonashecke/">
				<img class="h-5 w-5" src={linkedin} alt="linkedin_icon" />
			</a>
		</li>
	</ul>

	<div class="flex items-center justify-center h-32">
		<h1 class="text-2xl">Where to find us?</h1>
	</div>

	<div class="map mx-80">
		<Map {options} />
	</div>
</main>

<style>
	.map {
		height: 500px;
		width: auto;
	}
</style>
