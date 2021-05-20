<script>
  import Navbar from '../components/navbar.svelte';
  export let name;
</script>

<svelte:head>
	<title>Home</title>
</svelte:head>

<Navbar />

<main>
  <div class="py-32 text-center">
  <h2 class="font-extrabold text-4xl">Welcome to SvelteKit123</h2>
  <p class="text-2xl bg-blue-500"> 
      Test for Website
  </p> 
  <p>Visit <a class="text-blue-600 underline" href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>
  <p class="bg-green-200 font-sans-roboto font-semibold">A bias neuron allows for more variations of weights to be stored. Biases add richer representation of the input space to the model’s weights. In the case of neural networks, a bias neuron is added to every layer. It plays a vital role by making it possible to move the activation function to the left or right on the graph.
    </p> 
  </div>

  <div class="max-w-7xl px-32">
    <iframe width="500" height="280" src="https://www.youtube.com/embed/AllwTaOr_yw" title="Patient Reported Outcome Measures" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
  </div>
</main>

