<script>
	import logo from './heart.svg';
</script>

<nav class="bg-blue-100 text-lm">
	<div class="max-w-7xl mx-auto px-4">
		<div class="flex justify-between">
			<div class="flex space-x-12">
				<!-- logo-->
				<div>
					<a href="#" class="flex items-center py-3 px-2">
						<div class="h-12 w-12 mr-2">
							<img src={logo} alt="logo" />
						</div>
						<span class="font-bold text-blue-500">Healthspace</span>
					</a>
				</div>

				<!-- primary nav-->
				<div class="flex items-center space-x-1 text-gray-700">
					<a href="#" class="py-5 px-3 font-semibold text-gray-700 hover:text-blue-500">Blog</a>
					<a href="#" class="py-5 px-3 font-semibold text-gray-700 hover:text-blue-500">About</a>
				</div>
			</div>

			<!-- secondary nav-->
			<div class="flex items-center">
				<a href="" class="py-5 px-5">Login</a>
				<a href="" class="py-2 px-3 bg-purple-500 hover:bg-purple-400 text-white hover:text-white rounded transition duration-300">Signup</a>
			</div>

		</div>

		<!-- mobile menu-->
	</div>
</nav>
