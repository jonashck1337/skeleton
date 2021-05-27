<script>
	import logo from './heart.svg';
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
				</div>
			</div>

			<!-- right nav elements-->
			<div class="flex items-center text-gray-700">
				<a href="./login" class="py-5 px-5 font-semibold hover:text-blue-500">Login</a>
				<a href="./signup" class="py-2 px-3 bg-purple-500 hover:bg-purple-400 text-white hover:text-white rounded transition duration-300">Signup</a>
			</div>

		</div>

		<!-- mobile menu-->
	</div>
</nav>
