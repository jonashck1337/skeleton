<script>
  import Navbar from '../components/navbar.svelte';
  export let name;
</script>

<svelte:head>
	<title>Healthspace Home</title>
</svelte:head>

<Navbar />

<main>
  <div class="py-12 text-center">
  <p class="text-2xl bg-blue-500"> 
      Test for Website
  </p> 
  <p>Visit <a class="text-blue-600 underline" href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>
  <p class="bg-green-200 font-sans-roboto font-semibold">A bias neuron allows for more variations of weights to be stored. Biases add richer representation of the input space to the model’s weights. In the case of neural networks, a bias neuron is added to every layer. It plays a vital role by making it possible to move the activation function to the left or right on the graph.
    </p> 
  </div>

  <div class="flex justify-between items-start px-8">
    <div>
    <iframe width="550" height="280" src="https://www.youtube.com/embed/AllwTaOr_yw" title="Patient Reported Outcome Measures" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
  </div>
    <p class="ml-12 mr-8">The broad goal of clinical trials is to improve healthcare and its outcome for the population. By collecting patient reported outcome data, researchers get a brief insight into the frequency and variety of symptoms as well as the disease’s actual impact on daily life. These findings can later be used to close the gap between clinical research and therapy to ensure a patient-centered and high-quality care practice In the past, surveys have been administered on paper, which requires tedious administration and logistics, and can also pose a private health information security risk. Thanks to advancement in digital technology, it is now possible for researchers to easily collect data electronically and in a secure way using tools like ePROs (electronic Patient Reported Outcomes) or eCOA. Patients can complete secure electronic surveys sent via email, saving time, increasing engagement, and requiring less administration. At the moment, more than 26% of studies in Castor are using surveys.</p>
  </div>
</main>

