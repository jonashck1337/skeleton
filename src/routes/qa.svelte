<script>
    import Navbar from '../components/navbar.svelte';
    import Overlay from '../components/overlay.svelte';
    const qas = [
      {
        question: "What is Patient Reported Outcomes?",
        answer:
          "A patient-reported outcome (PRO) is a health outcome directly reported by the patient who experienced it. It stands in contrast to an outcome reported by someone else, such as a physician-reported outcome. PRO methods, such as forms, are used in clinical trials, to help better understand a treatment's efficacy or effectiveness. The use of digitized PROs, is on the rise in today's health research setting.",
      },
      {
        question: "Do I need to pay for this service?",
        answer:
          "Our service is completely free for patients. In order to support our operations, we will charge a fixed fee from your healthcare provider.",
      },
      {
        question: "How safe is my data?",
        answer:
          "We use our user data only to provide the services we have agreed upon, and for purposes that are compatible with providing those services. We do not share your data with our advertiser-supported services, nor do we mine it for marketing or advertising. If you leave the service, we take the necessary steps to ensure the continued ownership of your data.",
      },
      {
        question: "How often do I need to input data?",
        answer:
          "In order to avail the benefits of most accurate healthcare tracking services, we recommend you to fill your information on a weekly basis or as prescribed by your healthcare provider.",
      },
      {
        question: "What if I want to delete my account?",
        answer:
          "Our users always have an option to opt out of our service anytime they want. In this case, all the data related to the user will be deleted from our system within 30 days of account deletion.",
      },
      {
        question: "How can I contact you?",
        answer:
          "You can always contact us directly using the contact form above on this webpage.",
      },
    ];
    let group = qas[0];
  </script>
  
  <svelte:head>
    <title>Q&A</title>
  </svelte:head>
  

<Navbar />


<div class="px-72">
  <h2 class="font-bold text-2xl mt-20 mb-10 px-10">
    Most frequently asked questions:
  </h2>
  
  
  <div class="px-20">
    <div class="card mb-10 ">
      {#each qas as q, i}
        <Overlay name={q.question} bind:group>
          <div>
            {q.answer}
          </div>
        </Overlay>{/each}
    </div>
  </div>
  
  <h1 class="text-center text-4xl my-3 font-bold">Contact us</h1>
  <div class="px-20 my-10 ">
    <div class="flex justify-center flex-col px-20 py-15  card">
      <div>
        <span class="uppercase text-sm text-gray-600 font-bold">Full Name</span>
        <input
          class="w-full bg-gray-300 text-gray-900 mt-2 p-3 rounded-md focus:outline-none focus:shadow-outline"
          type="text"
          placeholder=""
        />
      </div>
      <div class="mt-8">
        <span class="uppercase text-sm text-gray-600 font-bold">Email</span>
        <input
          class="w-full bg-gray-300 text-gray-900 mt-2 p-3 rounded-md focus:outline-none focus:shadow-outline"
          type="text"
        />
      </div>
      <div class="mt-8">
        <span class="uppercase text-sm text-gray-600 font-bold">Message</span>
        <textarea
          class="w-full h-32 bg-gray-300 text-gray-900 mt-2 p-3 rounded-md focus:outline-none focus:shadow-outline"
        />
      </div>
      <div class="mt-8">
        <button
          class="uppercase text-sm font-bold tracking-wide bg-indigo-500 text-gray-100 p-3 rounded-md w-full focus:outline-none focus:shadow-outline"
        >
          Send Message
        </button>
      </div>
    </div>
  </div>
</div>

  <style>
    .card {
      border-radius: 4px;
      box-shadow: 0 3px 3px -2px rgba(0, 0, 0, 0.2),
        0 3px 4px 0 rgba(0, 0, 0, 0.14), 0 1px 8px 0 rgba(0, 0, 0, 0.12);
        padding:1em
    }
  </style>
  