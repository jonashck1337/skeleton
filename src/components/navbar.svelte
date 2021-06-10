<script>
	import logo from './heart.svg';
	import Modal from "./Modal.svelte";
	let modal;
</script>

<nav class="bg-blue-100 text-lm">
	<div class="max-w-8xl mx-auto px-8">
		<div class="flex justify-between">
			<div class="flex space-x-12">
				<!-- logo-->
				<div>
					<a href="." class="flex items-center py-3 px-2">
						<div class="h-12 w-12 mr-2">
							<img src={logo} alt="logo" />
						</div>
						<span class="font-bold text-blue-500">Healthspace</span>
					</a>
				</div>

				<!-- left nav elements-->
				<div class="flex items-center space-x-1 text-gray-700 font-semibold">
					<a href="./qa" class="py-5 px-3 hover:text-blue-500">Q&A</a>
					<a href="./about" class="py-5 px-3  hover:text-blue-500">About</a>
					<a href="/careers" class="py-5 px-3  hover:text-blue-500">Careers</a>
				</div>
			</div>

			  <!-- right nav elements-->
			  <div class="flex items-center text-gray-700 z-50">
				<button on:click={() => modal.show()} class="inline-block p-2 text-blue hover:text-blue-400 mr-2 font-bold">Login</button>
				<Modal bind:this={modal}>
					<div class="bg-white shadow-md rounded px-8 pt-6 pb-8 mb-4 flex flex-col">
						<div class="mb-4">
						  <label class="block text-grey-darker text-sm font-bold mb-2" for="username">
							Username
						  </label>
						  <input class="shadow appearance-none border rounded w-full py-2 px-3 text-grey-darker" id="username" type="text" placeholder="Username">
						</div>
						<div class="mb-6">
						  <label class="block text-grey-darker text-sm font-bold mb-2" for="password">
							Password
						  </label>
						  <input class="shadow appearance-none border border-red rounded w-full py-2 px-3 text-grey-darker mb-3" id="password" type="password" placeholder="******************">
						</div>
						<div class="flex items-center justify-between">
						  <button class="bg-blue-700 hover:bg-blue-dark text-white font-bold py-2 px-4 rounded" type="button">
							Sign In
						  </button>
						  <a class="inline-block align-baseline font-bold text-sm text-blue hover:text-blue-darker" href="#">
							Forgot Password?
						  </a>
						</div>
					</div>
				  <button on:click={() => modal.hide()}>Close</button>
				</Modal>
				<a href="/signup" class="py-2 px-3 bg-purple-500 hover:bg-purple-400 text-white hover:text-white rounded transition duration-300">Signup</a>
			</div>
		  </div>
	  </div>
  </nav>