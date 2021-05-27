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

    <div class="LI-profile-badge"  data-version="v1" data-size="large" data-locale="en_US" data-type="vertical" data-theme="light" data-vanity="lawrencesnow"><a class="LI-simple-link" href="https://www.linkedin.com/in/lawrencesnow?trk=profile-badge">Lawrence Snow</a></div>
    <div class="LI-profile-badge"  data-version="v1" data-size="large" data-locale="en_US" data-type="vertical" data-theme="light" data-vanity="jonashecke"><a class="LI-simple-link" href="https://www.linkedin.com/in/jonashecke?trk=profile-badge">Jonas Hecke</a></div>

    <div class="flex items-center justify-center h-32">
        <h1 class= "text-2xl">Where to find us?</h1>
    </div>

	<div class="map mx-80">
        <Map {options} />
      </div>
</main>