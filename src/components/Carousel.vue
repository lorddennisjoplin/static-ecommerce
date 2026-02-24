<template>
	<section id="carousel" class="my-5">
		<div class="container">
			<div class="row">
				<div class="col-12 col-lg-3">
					<div id="carouselExampleIndicators" class="carousel slide" data-bs-ride="carousel">
						<div class="carousel-indicators">
							<button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="0" class="active"></button>
							<button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="1"></button>
							<button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="2"></button>
						</div>

						<div class="carousel-inner">
							<div class="carousel-item active">
								<img class="d-block w-100" src="../../images/album-ex.jpg" alt="EX">
							</div>
							<div class="carousel-item">
								<img class="d-block w-100" src="../../images/album-duh.png" alt="DUH!">
							</div>
							<div class="carousel-item">
								<img class="d-block w-100" src="../../images/album-harmony-all-in.jpg" alt="Harmony: All In">
							</div>
						</div>

						<button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide="prev">
							<span class="carousel-control-prev-icon"></span>
							<span class="visually-hidden">Previous</span>
						</button>

						<button class="carousel-control-next" type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide="next">
							<span class="carousel-control-next-icon"></span>
							<span class="visually-hidden">Next</span>
						</button>
					</div>
				</div>
				<div class="col-12 col-lg-9 py-5 px-5">
					<h2 class="mb-4">Albums</h2>
					<p class="lead">Collecting P1Harmony albums? Here are all the available EPs, some of them even signed! With  fast shipping, great prices, and exceptional customer service.</p>
				</div>
			</div>
		</div>
	</section>
</template>

<script setup>
	import {defineProps} from 'vue';
	
	defineProps({
		project: Object
	})
</script>