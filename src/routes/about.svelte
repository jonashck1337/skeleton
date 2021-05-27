<script>
	import Navbar from '../components/navbar.svelte';
    import Map from '@anoram/leaflet-svelte';
        let options={
            center: [48.83407644724074,2.3716775921220727],
            markers: [
            {
            lat: 48.83407644724074,
            lng: 2.3716775921220727,
            },
        {
            lat: 48.83407644724074,
            lng: 2.3716775921220727,
                popup: {
                isOpen: true,
                text: `Healthspace @ Station F`,
        },
    },
    ],
        mapID: "map"
    };
    import Linkedin1 from './linkedin.svelte';
</script>

<svelte:head>
	<title>About</title>
</svelte:head>

<Navbar />

<style> 
    .map {
        height: 500px;
        width: auto;
      }</style>

<main>
	<div class="flex items-center justify-center h-32">
        <h1 class= "text-2xl">Who are we?</h1>
    </div>
    
    <div>
        <Linkedin1 />
    </div>

    <div class="flex items-center justify-center h-32">
        <h1 class= "text-2xl">Where to find us?</h1>
    </div>

	<div class="map mx-80">
        <Map {options} />
      </div>
</main>