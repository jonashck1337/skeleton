<script>
  import Navbar from '../components/navbar.svelte';
  import careers from '../components/careers.jpg';
</script>

<svelte:head>
  <title>Career</title>
</svelte:head>


<Navbar />

<div class="mx-48">
<section id="head" class="  my-15 py-15 grid grid-cols-1 md:grid-cols-2">
  <div class="p-8">
    <h1 class="text-5xl">
      Be part of the next revolution in healthcare. Join us as we scale
      internationally to help millions of patients benefit from better
      healthcare.
    </h1>
    <p class="text-1xl pt-4 text-justify">
      At Healthspace we have a talented team who are passionate about finding the
      best solutions to put the patient’s perspective at the center of
      healthcare. We are a diverse group of designers, engineers,
      scientists, thinkers and doers from different backgrounds working together
      to tackle big challenges.
    </p>
  </div>
  <div class="p-8">
    <img src={careers} alt="careers" />
  </div>
</section>

<section id="positions" class="my-1">
  <div class="d-flex padded_strike">
    <div class="flex-fill strikethrough d-flex" />
    <div class="d-block d-lg-inline-flex title strikethrough">
      Open Positions
    </div>
    <div class="flex-fill strikethrough d-flex" />
  </div>
  <p class="text-center p-10 mb-5">
    We are looking for exceptional problem-solvers to join our team. If you
    share our values and want to work in an innovative and stimulating
    environment, we want to hear from you.
  </p>
  <div class="flex flex-col  px-20 justify-center px-5">
    <div
      class="pt-4 pb-6 border-b-2  border-black gap-x-8 gap-y-4 grid  grid-cols-1 md:grid-cols-3"
    >
      <p class="font-bold">Frontend Engineer (d/f/m)</p>
      <p>Medical Affairs</p>
      <p>Paris</p>
    </div>

    <div
      class="pt-4 pb-6  border-b-2  border-black gap-x-8 gap-y-4  grid grid-cols-1 md:grid-cols-3"
    >
      <p class="font-bold">Senior Product Manager (d/f/m)</p>
      <p>Product</p>
      <p>Paris / remote </p>
    </div>

    <div
      class="pt-4 pb-6  border-b-2  border-black gap-x-8 gap-y-4 grid  grid-cols-1 md:grid-cols-3"
    >
      <p class="font-bold">Business Development Manager (d/f/m)</p>
      <p>Marketing</p>
      <p>Paris</p>
    </div>
  </div>
</section>

<section id="why-join-us" class="grid grid-cols-1 my-4 py-4 md:grid-cols-2">
  <div class="p-4">
    <h1 class="text-5xl">
      We are proud to provide a supportive and engaging work environment where
      our team members can employ their unique talents to really make a
      difference in the world.
    </h1>
  </div>
  <div class="p-8">
    <div class="flex flex-col">
      <div
        class="pt-4 pb-6 border-b-2  border-black gap-x-8 gap-y-4 grid  grid-cols-1 md:grid-cols-2"
      >
        <div class="icon">
          <img src="https://img.icons8.com/bubbles/100/000000/geography.png" alt="earth globe" />
        </div>
        <div>
          <h4 class="font-bold">Great Location</h4>
          <p>
            Our offices are located in the heart of the European startup scene
            with one in Paris Station F tower (more information in the about page).
          </p>
        </div>
      </div>

      <div
        class="pt-4 pb-6  border-b-2  border-black gap-x-8 gap-y-4  grid grid-cols-1 md:grid-cols-2"
      >
        <div class="icon" ><img src="https://img.icons8.com/dusk/64/000000/idea-bank.png" alt='piggy bank'/></div>
        <div>
          <h4 class="font-bold">Competitive Remuneration</h4>
          <p>
            We value the contributions of our team members and seek to
            compensate them accordingly.
          </p>
        </div>
      </div>

      <div
        class="pt-4 pb-6  border-b-2  border-black gap-x-8 gap-y-4 grid  grid-cols-1 md:grid-cols-2"
      >
        <div class="icon"><img src="https://img.icons8.com/officel/80/000000/teams.png" alt="team shirt"/></div>
        <div>
          <h4 class="font-bold">Team events</h4>
          <p>
            We would not be where we are today if our team did not know and
            trust one another. We regularly take time out of our schedule to
            learn from and check-in with one another. We also have regular team
            dinners and sports events.
          </p>
        </div>
      </div>

      <div
      class="pt-4 pb-6 border-b-2  border-black gap-x-8 gap-y-4 grid  grid-cols-1 md:grid-cols-2"
    >
      <div class="icon">
        <img src="https://img.icons8.com/nolan/96/critical-thinking.png" alt='brain'/>
      </div>
      <div>
        <h4 class="font-bold">Learning & Development</h4>
        <p>
          We are a high growth startup with ambitious goals. We believe that when our team members grow, the company grows too. We foster a work environment where everyone is encouraged to take time to learn new things and take on more responsibilities. We also give you time to think outside of the box and explore new ways to make things happen.
        </p>
      </div>
    </div>

    <div
    class="pt-4 pb-6 border-b-2  border-black gap-x-8 gap-y-4 grid  grid-cols-1 md:grid-cols-2"
  >
    <div class="icon">
      <img src="https://img.icons8.com/dusk/64/000000/3d-printer.png" alt='equipment'/>
    </div>
    <div>
      <h4 class="font-bold">Equipment      </h4>
      <p>
        And finally, you can choose whether you wish to work on a PC or Mac (MacBook Pro).
      </p>
    </div>
  </div>
    </div>
  </div>
</section>

<section id="positions" class=" my-15 py-15">
  <p class="text-center font-bold px-10 mb-5">
    If you have any questions, please do not hesitate to contact us also via:
  </p>
  <div class="flex justify-center">
    <button
      class=" hover:bg-blue-700 text-white font-bold py-2 px-4 rounded  bg-indigo-500 text-gray-100 p-3"
    >
      contact@websitecreation.essec.edu
    </button>
  </div>
</section>
</div>


<style>
  .padded_strike .strikethrough {
    border-bottom-width: 2px;
    border-bottom-style: solid;
  }
  .flex-fill {
    -ms-flex: 1 1 auto !important;
    flex: 1 1 auto !important;
  }
  .d-flex {
    display: -ms-flexbox !important;
    display: flex !important;
  }
  .flex-fill {
    -ms-flex: 1 1 auto !important;
    flex: 1 1 auto !important;
  }
  .d-flex {
    display: -ms-flexbox !important;
    display: flex !important;
  }

  .padded_strike .title {
    text-align: center;
    border: none;
    padding: 12px 30px;
    margin-bottom: -21px;
    font-weight: 700;
  }

  section:not(:last-of-type) {
    min-height: 540px;
    align-items: center;

    justify-content: center;
    flex-direction: column;
  }

  section:last-of-type{
    min-height: 200px;
    padding: 2em 0;
  }

  .icon {
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
  }
</style>
