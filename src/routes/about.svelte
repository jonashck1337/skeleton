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
		<h1 class="text-3xl">The team behind Healthspace</h1>
	</div>

	<ul class="flex justify-center space-x-12">
		<li>
			<a href="#">
				<img class="h-48 w-48 rounded-full" src={photo3} alt="Antoine" />
			</a>
            <a class="flex flex-col items-center py-3 font-semibold text-lg text-blue-500">Antoine Chauvin</a>
            <a class="flex flex-col items-center py-1" href="https://www.linkedin.com/in/antoine-chauvin-38b86b154/">
				<img class="h-5 w-5" src={linkedin} alt="linkedin_icon" />
			</a>
		</li>
        <li>
			<a href="#">
				<img class="h-48 w-48 rounded-full" src={photo4} alt="Inès" />
			</a>
            <a class="flex flex-col items-center py-3 font-semibold text-lg text-blue-500">Inès Mebarki</a>
            <a class="flex flex-col items-center py-1" href="https://www.linkedin.com/in/in%C3%A8s-mebarki/">
				<img class="h-5 w-5" src={linkedin} alt="linkedin_icon" />
			</a>
		</li>
        <li>
			<a href="#">
				<img class="h-48 w-48 rounded-full" src={photo2} alt="Raghav" />
			</a>
            <a class="flex flex-col items-center py-3 font-semibold text-lg text-blue-500">Raghav Bansal</a>
            <a class="flex flex-col items-center py-1" href="https://www.linkedin.com/in/raghavbansal/">
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

<div class="flex items-center justify-center h-32 text-3xl pt-32 pb-8">
<a>Our story</a>
</div>

	<div class="container mx-auto w-full h-full">
		<div class="relative wrap overflow-hidden p-10 h-full">
		  <div class="border-2-2 absolute border-opacity-20 border-gray-700 h-full border" style="left: 50%"></div>
		  <!-- right timeline -->
		  <div class="mb-8 flex justify-between items-center w-full">
			<div class="order-1 w-5/12"></div>
			<div class="z-20 flex items-center order-1 bg-gray-800 shadow-xl w-16 h-16 rounded-full">
			  <h1 class="mx-auto font-semibold text-lg text-white">1</h1>
			</div>
			<div class="order-1 bg-gray-400 rounded-lg shadow-xl w-5/12 px-6 py-4">
			  <h3 class="mb-3 font-bold text-gray-800 text-xl">2016</h3>
			  <p class="text-sm leading-snug tracking-wide text-gray-900 text-opacity-100">Healthpace was founded by the beatiful founding team.</p>
			</div>
		  </div>
	  
		  <!-- left timeline -->
		  <div class="mb-8 flex justify-between flex-row-reverse items-center w-full">
			<div class="order-1 w-5/12"></div>
			<div class="z-20 flex items-center order-1 bg-gray-800 shadow-xl w-8 h-8 rounded-full">
			  <h1 class="mx-auto text-white font-semibold text-lg">2</h1>
			</div>
			<div class="order-1 bg-red-400 rounded-lg shadow-xl w-5/12 px-6 py-4">
			  <h3 class="mb-3 font-bold text-white text-xl">2017</h3>
			  <p class="text-sm font-medium leading-snug tracking-wide text-white text-opacity-100">The first 1000 patients were registered on the platform.</p>
			</div>
		  </div>
		  
		  <!-- right timeline -->
		  <div class="mb-8 flex justify-between items-center w-full">
			<div class="order-1 w-5/12"></div>
			<div class="z-20 flex items-center order-1 bg-gray-800 shadow-xl w-8 h-8 rounded-full">
			  <h1 class="mx-auto font-semibold text-lg text-white">3</h1>
			</div>
			<div class="order-1 bg-gray-400 rounded-lg shadow-xl w-5/12 px-6 py-4">
			  <h3 class="mb-3 font-bold text-gray-800 text-xl">Lorem Ipsum</h3>
			  <p class="text-sm leading-snug tracking-wide text-gray-900 text-opacity-100">Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book.</p>
			</div>
		  </div>
	  
		  <!-- left timeline -->
		  <div class="mb-8 flex justify-between flex-row-reverse items-center w-full">
			<div class="order-1 w-5/12"></div>
			<div class="z-20 flex items-center order-1 bg-gray-800 shadow-xl w-8 h-8 rounded-full">
			  <h1 class="mx-auto text-white font-semibold text-lg">4</h1>
			</div>
			<div class="order-1 bg-red-400 rounded-lg shadow-xl w-5/12 px-6 py-4">
			  <h3 class="mb-3 font-bold text-white text-xl">Lorem Ipsum</h3>
			  <p class="text-sm font-medium leading-snug tracking-wide text-white text-opacity-100">Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book.</p>
			</div>
		  </div>
		</div>
	  </div>



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
