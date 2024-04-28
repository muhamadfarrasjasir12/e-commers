# e-commers

KELOMPOK:

Nama: Muhamad Farras Jasir

NIM: 312210361

Nama: Yehezkiel Juandro Metta

NIM: 312210376

KELAS: TI.22.A5


# Judul Open Trip Gunung


# database

Bagian database

-- phpMyAdmin SQL Dump

-- version 5.2.1

-- https://www.phpmyadmin.net/

--

-- Host: 127.0.0.1

-- Generation Time: Mar 20, 2024 at 08:11 PM

-- Server version: 10.4.28-MariaDB

-- PHP Version: 8.1.17

SET SQL_MODE = "NO_AUTO_VALUE_ON_ZERO";

START TRANSACTION;

SET time_zone = "+00:00";


/*!40101 SET @OLD_CHARACTER_SET_CLIENT=@@CHARACTER_SET_CLIENT */;

/*!40101 SET @OLD_CHARACTER_SET_RESULTS=@@CHARACTER_SET_RESULTS */;

/*!40101 SET @OLD_COLLATION_CONNECTION=@@COLLATION_CONNECTION */;

/*!40101 SET NAMES utf8mb4 */;

--
-- Database: `fravor`
--

-- --------------------------------------------------------

--
-- Table structure for table `admin`
--

CREATE TABLE `admin` (

  `id` int(11) NOT NULL,
  
  `username` varchar(255) NOT NULL,
  
  `password` varchar(255) NOT NULL

) 

ENGINE=InnoDB DEFAULT CHARSET=latin1 COLLATE=latin1_swedish_ci;

# Header

untuk bagian header

<!DOCTYPE html>
<html lang="en">
	<head>
		<meta charset="utf-8" />
		<title>Home Page</title>
		<meta content="width=device-width, initial-scale=1.0" name="viewport" />
		<meta content="" name="keywords" />
		<meta content="" name="description" />

		<!-- Lgo-->
		<link href=" <?php base_url() ?>../assets/img/logo/icon1.png" rel="icon" />

		<!-- Google Web Fonts -->
		<link rel="preconnect" href="https://fonts.googleapis.com" />
		<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
		<link
			href="https://fonts.googleapis.com/css2?family=Quicksand:wght@400;700&display=swap"
			rel="stylesheet"
		/>

		<!-- Icon Font Stylesheet -->
		<link
			href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.10.0/css/all.min.css"
			rel="stylesheet"
		/>
		<link
			href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.4.1/font/bootstrap-icons.css"
			rel="stylesheet"
		/>

		<!-- Libraries Stylesheet -->
		<link href=" <?php base_url() ?>../assets/lib/animate/animate.min.css" rel="stylesheet" />
		<link href=" <?php base_url() ?>../assets/lib/owlcarousel/assets/owl.carousel.min.css" rel="stylesheet" />

		<!-- Customized Bootstrap Stylesheet -->
		<link href=" <?php base_url() ?>../assets/css/bootstrap.min.css" rel="stylesheet" />
		
		<link rel="stylesheet" type="text/css" href="<?php base_url() ?>../assets/css/bootstrap.css">
    	<script type="text/javascript" src="js/jquery.js"></script>
    	<script type="text/javascript" src="js/bootstrap.js"></script>

		<!-- Template Stylesheet -->
		<link href=" <?php base_url() ?>../assets/css/style.css" rel="stylesheet" />
		<link rel="stylesheet" href=" <?php base_url() ?>../assets/css/font-awesome.css" />
		<link rel="stylesheet" href=" <?php base_url() ?>../assets/css/royal-preload.css" />
		<link rel="stylesheet" href=" <?php base_url() ?>../assets/css/owl.carousel.min.css" />
		<link rel="stylesheet" href=" <?php base_url() ?>../assets/css/font-awesome.css" />
		<link rel="stylesheet" href=" <?php base_url() ?>../assets/css/magnific-popup.css" />
	</head>

	<body>
		<!-- Spinner Start -->
		<div
			id="spinner"
			class="show bg-black position-fixed translate-middle w-100 vh-100 top-50 start-50 d-flex align-items-center justify-content-center"
		>
			<div class="spinner-grow text-primary" role="status"></div>
		</div>

		<!-- Spinner End -->

		
		<!-- Navbar Start -->
		<nav style="text-transform: lowercase;" class="navbar navbar-expand-lg bg-success navbar-light sticky-top p-0">
			<a
				href="<?php echo base_url()?>fravor/index"
				class="navbar-brand d-flex align-items-center border-end px-4 px-lg-5"
			>
				<img src=" <?php base_url() ?>../assets/img/logo/icon1.png" width="100px"/>
			</a>
			<button
				type="button"
				class="navbar-toggler me-4"
				data-bs-toggle="collapse"
				data-bs-target="#navbarCollapse"
			>
				<span class="navbar-toggler-icon"></span>
			</button>
			<div class="collapse navbar-collapse" id="navbarCollapse">
				<div class="navbar-nav ms-auto p-4 p-lg-0">
					<div class="nav-item dropdown">
						<a href="<?php echo base_url()?>fravor/index" class="nav-link">Home</a>
						<!-- <div class="dropdown-menu bg-light m-0">
							<a href="sejarah.html" class="dropdown-item">Sejarah</a>
							<a href="appointment.html" class="dropdown-item">Logo</a>
							<a href="team.html" class="dropdown-item">Visi Misi</a>
							<a href="testimonial.html" class="dropdown-item"
								>Struktur Organisai</a
							>
							<a href="404.html" class="dropdown-item"
								>Grand Desain HIMATIF 2022</a
							>
						</div> -->
					</div>
					<div class="nav-item dropdown">
						<a href="<?php echo base_url()?>fravor/wisata" class="nav-link">Wisata</a>
						
					</div>	

					<div class="nav-item dropdown">
					<a href="<?php echo base_url()?>fravor/booking" class="nav-link"
						>booking</a
						>
					</div>
					<div class="nav-item dropdown">
						<a
							href="#"
							class="nav-link dropdown-toggle"
							style="text-transform: capitalize;"
							data-bs-toggle="dropdown"
							>Galeri</a
						>
						<div class="dropdown-menu bg-light m-0">
							<!-- <a href="<?php echo base_url(). 'himatif/pm' ?>" class="dropdown-item" style="text-transform: capitalize;">Penjamin Mutu</a> -->
							
							<a href="<?php echo base_url()?>fravor/booking" class="dropdown-item" style="text-transform: capitalize;"
								>Pengembangan Organisasi</a
							>
							<a href="<?php echo base_url()?>himatif/medkom" class="dropdown-item" style="text-transform: capitalize;"
								>Media dan Komunikasi</a
							>
							<a href="<?php echo base_url()?>himatif/miba" class="dropdown-item" style="text-transform: capitalize;"
								>Minat dan Bakat</a
							>
							<a href="<?php echo base_url()?>himatif/litbang" class="dropdown-item" style="text-transform: capitalize;"
								>Penelitan dan Pengembangan</a
							>
							<a href="<?php echo base_url()?>himatif/hubin" class="dropdown-item" style="text-transform: capitalize;">HUBIN HUBEKS</a>
						</div>
							<!-- <a href="appointment.html" class="dropdown-item" style="text-transform: capitalize;">Workshop</a> -->
						</div>
					</div>
					<!-- <a href="contact.html" class="nav-item nav-link" style="text-transform: capitalize;">Contact</a> -->
				</div>
				<a href="<?php echo base_url()?>login/admin" class="btn btn-light py-4 px-lg-5 d-none d-lg-block" style="text-transform: capitalize;"
					>Login<i class="bi bi-door-open ms-3" ></i
				></a>
			</div>
		</nav>
		<!-- Navbar End -->

  
# Footer

untuk bagian footer

<!-- Footer Start -->
<div class="container-fluid bg-success text-light footer my-6 mb-0 py-6 wow fadeIn"
			data-wow-delay="0.1s">
			<div class="container">
				<div class="row g-7">
					<div class="col-lg-4 col-md-6">
						<h2 class="text-primary mb-4">
							<i></i>FRAVOR
						</h2>
						<p class="mb-2">
							<i class="fa fa-map-marker-alt me-3"></i>Jl. KPG.Selang Cironggeng, Wanajaya, Kec.Cibitung, Kabupaten Bekasi, Jawa Barat 17520
						</p>
						<p class="mb-2">
							<i class="fa fa-phone-alt me-3"></i>089519649447
						<p class="mb-2">
							<i class="fa fa-envelope me-3"></i>fravor12@gmail.com
						</p>
					</div>
					<div class="col-lg-4 col-md-8">
						<h4 class="text-primary mb-4">Quick Links</h4>
						<a class="btn btn-link" href="">About Us</a>
						<a class="btn btn-link" href="">Contact Us</a>
						<a class="btn btn-link" href="">Our Services</a>
						<a class="btn btn-link" href="">Terms & Condition</a>
						<a class="btn btn-link" href="">Support</a>
					</div>
					
					<div class="col-lg-3 col-md-6">
						<!-- <h4 class="text-light mb-4">Newsletter</h4>
						<!--<form action="">-->
						<!--	<div class="input-group">-->
						<!--		<input-->
						<!--			type="text"-->
						<!--			class="form-control p-3 border-0"-->
						<!--			placeholder="Your Email Address"-->
						<!--		/>-->
						<!--		<button class="btn btn-primary">Sign Up</button>-->
						<!--	</div>-->
						<!--</form> -->
						<h6 class="text-primary mt-6 mb-3">Follow Us</h6>
						<div class="d-flex pt-2">
						
							<a class="btn btn-square btn-outline-light me-1" href=""
								><i class="fab fa-facebook-f"></i
							></a>
							<a class="btn btn-square btn-outline-light me-1" href="https://www.youtube.com/channel/UC7SGrlmtAaBh2XTPpSO2Gfg"
								><i class="fab fa-youtube"></i
							></a>
							<a class="btn btn-square btn-outline-light me-0" href="https://www.instagram.com/himatif_pb/?hl=id"
								><i class="fab fa-instagram"></i
							></a>
						</div>
					</br>
						<div class="col-lg-4 col-md-2 h-800 w-200">
							<a href="https://www.indowebsite.co.id/">
								<img src="<?php base_url() ?>../assets/img/images/iw.png" alt="" >

							</a>
						</div>
					</div>
				</div>
			</div>
		</div>
		
		<!-- Footer End -->

		<!-- Copyright Start -->
		<div
			class="copyright text-light py-0 wow fadeIn"
			data-wow-delay="0.1s">
			<div class="">
				<div class="row">
					<div class="col-md-6 text-center text-md-start mb-3 mb-md-0">
						&copy; <a href="#">FRAVOR</a>
					</div>
					<div class="col-md-6 text-center text-md-end">
						<i class="balloon-heart-fill"></i>
						<!--/*** This template is free as long as you keep the footer author’s credit link/attribution link/backlink. If you'd like to use the template without the footer author’s credit link/attribution link/backlink, you can purchase the Credit Removal License from "https://htmlcodex.com/credit-removal". Thank you for your support. ***/-->
						Designed By <a href="#">Muhamad Farras Jasir</a>
					
					</div>
				</div>
			</div>
		</div>
		<!-- Copyright End -->
		<!-- Back to Top -->
		<a href="#" class="btn btn-lg btn-primary btn-lg-square back-to-top"
			><i class="bi bi-arrow-up"></i
		></a>

		<!-- Back to Top -->
		<a href="#" class="btn btn-lg btn-primary btn-lg-square back-to-top"
			><i class="bi bi-arrow-up"></i
		></a>

		<!-- JavaScript Libraries -->
		<script src="https://code.jquery.com/jquery-3.4.1.min.js"></script>
		<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.0.0/dist/js/bootstrap.bundle.min.js"></script>
		<script src="<?php base_url() ?>../assets/lib/wow/wow.min.js"></script>
		<script src="<?php base_url() ?>../assets/lib/easing/easing.min.js"></script>
		<script src="<?php base_url() ?>../assets/lib/waypoints/waypoints.min.js"></script>
		<script src="<?php base_url() ?>../assets/lib/owlcarousel/owl.carousel.min.js"></script>

		<!-- Template Javascript -->
		<script src="<?php base_url() ?>../assets/js/main.js"></script>
		<script src="<?php base_url() ?>../assets/js/jquery.magnific-popup.min.js"></script>
		<script src="<?php base_url() ?>../assets/js/royal_preloader.min.js"></script>
		<script src="<?php base_url() ?>../assets/js/jquery.magnific-popup.min.js"></script>
		<script src="<?php base_url() ?>../assets/js/jquery.isotope.min.js"></script>
		<script src="<?php base_url() ?>../assets/js/easypiechart.js"></script>
		<script src="<?php base_url() ?>../assets/js/owl.carousel.min.js"></script>
		<script src="<?php base_url() ?>../assets/js/particles.min.js"></script>
	</body>
</html>
<script type="text/javascript">
	window.jQuery = window.$ = jQuery;
	(function ($) {
		"use strict";
		//Preloader
		Royal_Preloader.config({
			mode: "logo",
			logo: "<?php base_url() ?>../assets/img/logo/icon1.png",
			logo_size: [100, 95],
			showProgress: true,
			showPercentage: true,
			text_colour: "#000000",
			background: "#ffffff",
		});
	})(jQuery);
</script>

# Home

Bagian Home

<!-- Carousel Start -->
<div class="container-fluid p-0 wow fadeIn" data-wow-delay="0.1s">
			<div id="header-carousel" class="carousel slide" data-bs-ride="carousel bg">
				<div class="carousel-inner">
					<div class="carousel-item active">
						<img class="w-100 h-100" src="<?php base_url() ?>../assets/img/logo/g-rinjani.jpg" alt="Image" />
						<div class="carousel-caption">
							<div class="container">
								<div class="row justify-content-center">
									<div class="col-lg-7">
										<h1 class="display-2 text-light mb-5 animated slideInDown">
											Selamat Datang di Website Kami
										</h1>

										<div class="video-popup">
											<div class="btn-inner">
												<a
													class="btn-play"
													href=""
													><i class="fas fa-play"></i>
													<span class="circle-1"></span>
													<span class="circle-2"></span>
												</a>
												<h6>"Histoire De Ma Maison"</h6>
											</div>
										</div>
										<!-- <a href="" class="btn btn-primary py-sm-3 px-sm-5"
											>Learn More</a
										>
										<a href="" class="btn btn-light py-sm-3 px-sm-5 ms-3"
											>Our Courses</a
										> -->
									</div>
								</div>
							</div>
						</div>
					</div>
					<div class="carousel-item">
						<img class="w-100 h-100" src="<?php echo base_url() ?>assets/img/logo/g-rinjani.jpg" alt="Image2" />
						<div class="carousel-caption">
							<div class="container">
								<div class="row justify-content-center">
									<div class="col-lg-20">
										<div class="video-popup">
											<div class="btn-inner">
												<a
													class="btn-play"
													href="https://www.youtube.com/watch?v=Dnh1BFcV_2I"
													><i class="fas fa-play"></i>
													<span class="circle-1"></span>
													<span class="circle-2"></span>
												</a>
												<h6>"1"</h6>
											</div>
										</div>
										<!-- <a href="" class="btn btn-primary py-sm-3 px-sm-5"
											>Learn More</a
										>
										<a href="" class="btn btn-light py-sm-3 px-sm-5 ms-3"
											>Our Courses</a
										> -->
									</div>
								</div>
							</div>
						</div>
					</div>
				</div>
				<button
					class="carousel-control-prev"
					type="button"
					data-bs-target="#header-carousel"
					data-bs-slide="prev"
				>
					<span class="carousel-control-prev-icon" aria-hidden="true"></span>
					<span class="visually-hidden">bb</span>
				</button>
				<button
					class="carousel-control-next"
					type="button"
					data-bs-target="#header-carousel"
					data-bs-slide="next"
				>
					<span class="carousel-control-next-icon" aria-hidden="true"></span>
					<span class="visually-hidden">Next</span>
				</button>
			</div>
		</div>
		<!-- Carousel End -->

		<!-- Facts Start -->

		<!-- Facts End -->

		<!-- About Start -->
		<div class="container-xxl py-6">
			<div class="container">
				<div class="row g-5">
					<div class="col-lg-6 wow fadeInUp" data-wow-delay="0.1s">
						<div
							class="position-relative overflow-hidden ps-5 pt-5 h-100"
							style="min-height: 400px"
						>
							<img
								class="position-absolute w-100 h-100"
								src="<?php base_url() ?>../assets/img/logo/alam2.jpeg"
								alt=""
								style="object-fit: cover"
							/>
							<img
								class="position-absolute top-0 start-0 bg-white pe-3 pb-3"
								src="<?php base_url() ?>../assets/img/logo/icon1.png"
								alt=""
								style="width: 200px; height: 200px"
							/>
						</div>
					</div>
					<div class="col-lg-6 wow fadeInUp" data-wow-delay="0.5s">
						<div class="h-100">
							<h2 style="text-align: center">
								<span style="color: Blue"><b> Analisis Situasi </b></span>
							</h2>
							<!-- <h1 class="display-6 mb-4">
								We Help Students To Pass Test & Get A License On The First Try
							</h1> -->
							<p style="text-align: justify">
							<span class="text-center"style="color: black"><b>
							Analisis Situasi
Aktivitas pendakian gunung di Indonesia meningkat dalam lima tahun terakhir. Sayangnya, peningkatan itu justru menimbulkan dampak buruk, salah satunya volume sampah di gunung yang semakin besar. Hal ini menunjukkan para pendaki cenderung lebih fokus pada elemen aktivitas fisik, belum mementingkan elemen lainnya, yaitu lingkungan alam dan interaksi budaya.
								</b></span>
							</p>
							<p>
								<span class="text-center" style="color: black"
									><b> Manfaat dan Tujuan Pengembangan Prototype

Situs pendakian gunung EnsikloPendaki dibuat untuk memberikan informasi dan edukasi soal pendakian gunung kepada pendaki pemula. Informasi dan edukasi tersebut diharapkan dapat membuat pendaki pemula menjadi pendaki yang bertanggung jawab ketika melakukan aktivitas pendakian gunung. </b></span
								>
							</p>

							<p>
							<span class="text-center" style="color: black">
							<b>Prototype yang Dikembangkan

Situs pendakian gunung EnsikloPendaki memberikan pemahaman secara luas tentang aktivitas pendakian gunung kepada khalayak sasaran. Oleh karena itu, situs ini memuat berita terkini, informasi yang dibutuhkan dan ingin diketahui lebih jauh oleh khalayak sasaran, dan pembahasan soal pendakian gunung dari film, buku, atau tokoh. Khalayak sasaran yang dimaksud adalah pendaki pemula berusia 16-23 tahun dengan Status Sosial Ekonomi A dan B. </b>
							</p>	
							</span>
							

							<p>
								<span class="text-center" style="color: black"
									><b> Evaluasi

Pretes terhadap prototype situs pendakian gunung EnsikloPendaki dilakukan satu bulan sebelum peluncuran situs. Kemudian, evaluasi akan dilakukan secara berkala, meliputi input, output, dan outcome. Pretes dan evaluasi ini dilakukan untuk melihat kesesuaian konten dan tampilan situs dengan kebutuhan khalayak sasaran. </b></span
								>
							</p>

							<div class="row g-2 mb-4 pb-2">
								<div style="text-align: justify" class="col-sm-6">
									
								</div>
								<div style="text-align: justify" class="col-sm-6">
									
								</div>
								
							</div>
							<div class="row g-4">
								<div class="col-sm-6">
									<a
										class="btn btn-outline-dark py-3 px-5"
										style ="border-radius: 10px"
										href="https://www.youtube.com/watch?v=_Oqe7qaoE6Y"
										><span class="text-center" style="color: black"><b>Lihat Film Dukumenter</b></span></a
									>
								</div>
								<!-- <div class="col-sm-6">
									<a
										class="d-inline-flex align-items-center btn btn-outline-primary border-2 p-2"
										href="NoHp:08777536521"
									>
										<span class="flex-shrink-0 btn-square bg-primary">
											<i class="fa fa-phone-alt text-white"></i>
										</span>
										<span class="px-3">087775365921</span>
									</a>
								</div> -->
							</div>
						</div>
					</div>
				</div>
			</div>
		</div>
		
		<!-- Features End -->
		

		<!-- Department -->
		<div class="container-xxl py-6">
			<div class="container">
				<div
					class="text-center mx-auto mb-5 wow fadeInUp"
					data-wow-delay="0.1s"
					style="max-width: 500px"
				>
					<h1 class="display-6 mb-4"></h1>
				</div>
				<div class="row g-0 team-items">
				
					<div class="col-lg-4 col-md-6 wow fadeInUp" data-wow-delay="0.1s">
						<div class="team-item position-relative">
							<div class="position-relative">
								<img class="img-fluid" src="<?php echo base_url(). 'assets/img/images/dpt/.png' ?>" alt="" />
								<div class="team-social text-center">
									<a
										class="btn btn-square btn-outline-primary border-2 m-1"
										href="<?php echo base_url(). 'himatif/po' ?>"
										>
									</a>
								</div>
							</div>
							
						</div>
					</div>
			
					
					<div class="col-lg-4 col-md-5 wow fadeInUp" data-wow-delay="0.3s">
						<div class="team-item position-relative">
							<div class="position-relative">
								<img class="img-fluid" src="<?php echo base_url(). 'assets/img/images/dpt/png' ?>" alt="" />
								<div class="team-social text-center">
									<a
										class="btn btn-square btn-outline-primary border-2 m-1"
										href="<?php echo base_url(). 'fravor/medkom' ?>"
										>
									</a>
								</div>
							</div>
							
						</div>
					</div>
					

					<div class="col-lg-4 col-md-6 wow fadeInUp" data-wow-delay="0.5s">
						<div class="team-item position-relative">
							<div class="position-relative">
								<img class="img-fluid" src="<?php echo base_url(). 'assets/img/images/dpt/.png' ?>" alt="" />
								<div class="team-social text-center">
									<a
										class="btn btn-square btn-outline-primary border-2 m-1"
										href="<?php echo base_url(). 'fravor/miba' ?>"
										><i class="bi bi-hand-index-fill"></i
									></a>
								</div>
							</div>
							
						</div>
					</div>
				
					<!-- Pembatas -->
					<div class="col-lg-1 col-md-6 wow fadeInUp" data-wow-delay="0.7s">	
					</div>
                 
                    <!-- End -->
					<div class="col-lg-4 col-md-6 wow fadeInUp" data-wow-delay="0.7s">
						<div class="team-item position-relative">
							<div class="position-relative">
								<img class="img-fluid" src="<?php base_url() ?>../assets/img/images/dpt/.png" alt="" />
								<div class="team-social text-center">
									<a
										class="btn btn-square btn-outline-primary border-2 m-1"
										href="<?php echo base_url(). 'fravor/litbang' ?>"
										><i class="bi bi-hand-index"></i
									></a>
								</div>
							</div>
							
						</div>
					</div>
					<!-- Pembatas -->
					<div class="col-lg-1 col-md-6 wow fadeInUp" data-wow-delay="0.7s">	
					</div>
					

					<div class="col-lg-4 col-md-6 wow fadeInUp" data-wow-delay="0.7s">
						<div class="team-item position-relative">
							<div class="position-relative">
								<img class="img-fluid" src="<?php echo base_url(). 'assets/img/images/dpt/.png' ?>" alt="" />
								<div class="team-social text-center">
									<a
										class="btn btn-square btn-outline-primary border-2 m-1"
										href="<?php echo base_url(). 'fravor/hubin' ?>"
										><i class="bi bi-hand-index-fill"></i
									></a>
								</div>
							</div>
							
						</div>
					</div>
				</div>
			</div>
		</div>

		<!-- Start Event -->

		<!-- Event Start -->
		<div class="container">		
        	<center><h1>Galeri Kegiatan</h1></center>
        	<br/>
        	<div>
        		<div id="myCarousel" class="carousel slide" data-ride="carousel">
        			<!-- Indicators -->
        			<ol class="carousel-indicators">
        				<li data-target="#myCarousel" data-slide-to="0" class="active"></li>
        				<li data-target="#myCarousel" data-slide-to="1"></li>
        				<li data-target="#myCarousel" data-slide-to="2"></li>		
        			</ol>
         
        			<!-- deklarasi carousel -->
        			<div class="carousel-inner" role="listbox">
        				<div class="item active">
        					<img src="<?php echo base_url(). 'assets/img/images/dpt/L5.png' ?>" alt="www.malasngoding.com">
        					<div class="carousel-caption">
        						<h3>1</h3>
        						<p>2.</p>
        					</div>
        				</div>
        				<div class="item">
        					<img src="img/malasngoding2.png" alt="www.malasngoding.com">
        					<div class="carousel-caption">
        						<h3>1</h3>
        						<p>1</p>
        					</div>
        				</div>
        				<div class="item">
        					<img src="img/malasngoding3.png" alt="www.malasngoding.com">
        					<div class="carousel-caption">
        						<h3>1</h3>
        						<p>2.</p>
        					</div>
        				</div>				
        			</div>
         
        			<!-- membuat panah next dan previous -->
        			<a class="left carousel-control" href="#myCarousel" role="button" data-slide="prev">
        				<span class="glyphicon glyphicon-chevron-left" aria-hidden="true"></span>
        				<span class="sr-only">Previous</span>
        			</a>
        			<a class="right carousel-control" href="#myCarousel" role="button" data-slide="next">
        				<span class="glyphicon glyphicon-chevron-right" aria-hidden="true"></span>
        				<span class="sr-only">Next</span>
        			</a>
        		</div>
        	</div>
           </div>
        		
		<!-- event End -->
		
	
		
<!-- Saran -->
		<div class="container-xxl py-6">
			<div class="container">
				<div class="row g-5">
					<div class="col-lg-6 wow fadeInUp" data-wow-delay="0.1s">
						<div
							class="position-relative overflow-hidden ps-5 pt-5 h-100"
							style="min-height: 400px"
						>
							<img
								class="position-absolute w-100 h-100"
								src="<?php echo base_url(). 'assets/img/proker/kotakaspirasi.png' ?>" alt=""
								style="object-fit: cover"
							/>
							<!-- <img
								class="position-absolute top-0 start-0 bg-white pe-3 pb-3"
								src="<?php echo base_url(). 'assets/img/logo/him.png' ?>" alt=""
								style="width: 200px; height: 200px"
							/> -->
						</div>
					</div>
					<div class="col-lg-6 wow fadeInUp" data-wow-delay="0.5s">
						<h4 class="text-dark text-uppercase mb-2 " style="text-align: center;" >Saran</h4>
						<!-- <h6 class="display-8 mb-4">
							Silahkan kirimkan kami sebuah saran
						</h6> -->
						<p class="mb-4">
							Hallo jika kalian mempunyai saran tentang keluh kesah dalam akademik silahkan kirimkaan keluh kesah kalian, jangan sungkan.
							<a href="https://dirmawa.pelitabangsa.ac.id/bimbingan-konseling/">Bimbingan Konseling</a>
						</p>
						<form>
							<div class="row g-3">
								<div class="col-md-6">
									<div class="form-floating">
										<input
											type="text"
											class="form-control border-0 bg-light"
											id="name"
											placeholder="Your Name"
										/>
										<label for="name">Your Name</label>
									</div>
								</div>
								<div class="col-md-6">
									<div class="form-floating">
										<input
											type="email"
											class="form-control border-0 bg-light"
											id="email"
											placeholder="Your Email"
										/>
										<label for="email">Your Email</label>
									</div>
								</div>
								<div class="col-12">
									<div class="form-floating">
										<input
											type="text"
											class="form-control border-0 bg-light"
											id="subject"
											placeholder="Subject"
										/>
										<label for="subject">Subject</label>
									</div>
								</div>
								<div class="col-12">
									<div class="form-floating">
										<textarea
											class="form-control border-0 bg-light"
											placeholder="Leave a message here"
											id="message"
											style="height: 150px"
										></textarea>
										<label for="message">Message</label>
									</div>
								</div>
								<div class="col-12">
									<button class="btn btn-success py-3 px-5" type="submit">
										Send Message
									</button>
								</div>
							</div>
						</form>
					</div>
					</div>
			</div>
		</div>
		<!-- Contact End -->

  # Wisata

  Bagian wisata

  
	<body>

		<!-- Page Header Start -->
		
		<!-- Page Header End -->

		
							<!-- <div class="col-sm-6 wow fadeIn" data-wow-delay="0.4s">
                            <div class="d-flex align-items-center mb-3">
                                <div class="flex-shrink-0 btn-square bg-primary me-3">
                                    <i class="fa fa-check text-white"></i>
                                </div>
                                <h5 class="mb-0">Best Trainers</h5>
                            </div>
                            <span>Magna sea eos sit dolor, ipsum amet ipsum lorem diam eos</span>
                        </div> -->
					
		<!-- Features End -->
		<!-- Team Start -->
		<div class="container-xxl py-7">
			<div class="container">
				<div
					class="text-center mx-auto mb-5 wow fadeInUp"
					data-wow-delay="0.1s"
					style="max-width: 500px"
				>
					<h2 class="display-4 mb-20">Wisata Alam</h2>
					<h6 class="text-primary text-uppercase mb-2"></h6>
				</div>
				<div class="row g-0 team-items">
					<!-- Pembatas -->
					<div class="col-lg-1 col-md-6 wow fadeInUp" data-wow-delay="0.7s">	
					</div>
                    <div class="col-lg-1 col-md-6 wow fadeInUp" data-wow-delay="0.7s">
					</div>
                    <!-- End -->
					<div class="col-lg-10 col-md-6 wow fadeInUp" data-wow-delay="0.5s">
						
					</div>

					<!-- Pembatas -->					

					<div class="col-lg-3 col-md-6 wow fadeInUp" data-wow-delay="0.7s">
						<div class="team-item position-relative">
							<div class="position-relative">
								<img
									class="img-fluid"
									src="<?php base_url() ?>../assets/img/logo/g-rinjani.jpg"
									alt=""
								/>
								<div class="team-social text-center">
									<a
										class="btn btn-square btn-outline-primary border-2 m-1"
										href=""
										><i class="fab fa-facebook-f"></i
									></a>
									<a
										class="btn btn-square btn-outline-primary border-2 m-1"
										href=""
										><i class="fab fa-twitter"></i
									></a>
									<a
										class="btn btn-square btn-outline-primary border-2 m-1"
										href=""
										><i class="fab fa-instagram"></i
									></a>
								</div>
							</div>
							<div class="bg-light text-center p-3">
								<p> Gunung Rinjani adalah gunung yang berlokasi di pulau lombok, (NTB) mempunyai ketinggia 3.726mdpl.</p>
								<div class="bg-success text-center p-3">
									<a href="<?php echo base_url()?>fravor/booking">Lihat Selengkapnya</a>
								</div>
							</div>
						</div>
					</div>

					<div class="col-lg-3 col-md-6 wow fadeInUp" data-wow-delay="0.7s">
						<div class="team-item position-relative">
							<div class="position-relative">
								<img
									class="img-fluid"
									src="<?php base_url() ?>../assets/img/logo/kerinci1.jpg"
									alt=""
								/>
								<div class="team-social text-center">
									<a
										class="btn btn-square btn-outline-primary border-2 m-1"
										href=""
										><i class="fab fa-facebook-f"></i
									></a>
									<a
										class="btn btn-square btn-outline-primary border-2 m-1"
										href=""
										><i class="fab fa-twitter"></i
									></a>
									<a
										class="btn btn-square btn-outline-primary border-2 m-1"
										href=""
										><i class="fab fa-instagram"></i
									></a>
								</div>
							</div>
							<div class="bg-light text-center p-3">
								<p>Gunung Kerinci adalah gunung tertinggi di pulau sumatra mempunyai ketinggian 3.805mdpl</p>
								<div class="bg-success text-center p-3">
									<a href="<?php echo base_url()?>fravor/booking">Lihat Selengkapnya</a>
								</div>
							</div>
						</div>
					</div>

					<div class="col-lg-3 col-md-6 wow fadeInUp" data-wow-delay="0.7s">
						<div class="team-item position-relative">
							<div class="position-relative">
								<img
									class="img-fluid"
									src="<?php base_url() ?>../assets/img/logo/semeru.png"
									alt=""
								/>
								<div class="team-social text-center">
									<a
										class="btn btn-square btn-outline-primary border-2 m-1"
										href=""
										><i class="fab fa-facebook-f"></i
									></a>
									<a
										class="btn btn-square btn-outline-primary border-2 m-1"
										href=""
										><i class="fab fa-twitter"></i
									></a>
									<a
										class="btn btn-square btn-outline-primary border-2 m-1"
										href=""
										><i class="fab fa-instagram"></i
									></a>
								</div>
							</div>
							<div class="bg-light text-center p-3">
								<p>Gunung semeru merupakan gunung tertinggi di pulau jawa, dengan puncaknya Mahameru 3.676</p>
								<div class="bg-success text-center p-3">
									<a href="<?php echo base_url()?>booking">Lihat Selengkapnya</a>
								</div>
							</div>
						</div>
					</div>
					
					<div class="col-lg-3 col-md-6 wow fadeInUp" data-wow-delay="0.7s">
						<div class="team-item position-relative">
							<div class="position-relative">
								<img
									class="img-fluid"
									src="<?php base_url() ?>../assets/img/logo/argopuro2.jpg"
									alt=""
								/>
								<div class="team-social text-center">
									<a
										class="btn btn-square btn-outline-primary border-2 m-1"
										href=""
										><i class="fab fa-facebook-f"></i
									></a>
									<a
										class="btn btn-square btn-outline-primary border-2 m-1"
										href=""
										><i class="fab fa-twitter"></i
									></a>
									<a
										class="btn btn-square btn-outline-primary border-2 m-1"
										href=""
										><i class="fab fa-instagram"></i
									></a>
								</div>
							</div>
							<div class="bg-light text-center p-3">
								<p>Gunung Argopuro berada di jawa timur dan mempunyai ketinggian 3.088mdpl</p>
								<div class="bg-success" text-center p-3>
								<a href="<?php base_url()?>booking" class="nav-link">Lihat selengkapnya</a>
								</div>
							</div>
						</div>
					</div>

					<div class="col-lg-3 col-md-6 wow fadeInUp" data-wow-delay="0.7s">
						<div class="team-item position-relative">
							<div class="position-relative">
								<img
									class="img-fluid"
									src="<?php base_url() ?>../assets/img/logo/ciremai.jpg"
									alt=""
								/>
								<div class="team-social text-center">
									<a
										class="btn btn-square btn-outline-primary border-2 m-1"
										href=""
										><i class="fab fa-facebook-f"></i
									></a>
									<a<div class="container-fluid p-0 wow fadeIn" data-wow-delay="0.1s">
			<div id="header-carousel" class="carousel slide" data-bs-ride="carousel bg">
				<div class="carousel-inner">
					<div class="carousel-item active">
						<img class="w-100 h-100" src="<?php base_url() ?>../assets/img/logo/g-rinjani.jpg" alt="Image" />
						<div class="carousel-caption">
							<div class="container">
								<div class="row justify-content-center">
								<div class="bg-success text-center p-3">
								<p> Booking Gunung Rinjani</p>
								<div class="bg-success text-center p-3">
									<a href="<?php echo base_url()?>panduan_booking"></a>
        							<form method="post">
        								<label for="tanggal">Tanggal:</label>
        								<input type="text" name="tanggal" id="tanggal" required>
        								<br><br>
        								<label for="bulan">Bulan:</label>
        								<input type="text" name="bulan" id="bulan" required>
        								<br><br>
        								<label for="tahun">Tahun:</label>
        								<input type="text" name="tahun" id="tahun" required>
        								<br><br>
        								<input type="submit" name="submit" value="Submit">
    								</form>

    								<?php
    								if (isset($_POST['submit'])) {
        							$tanggal = $_POST['tanggal'];
        							$bulan = $_POST['bulan'];
        							$tahun = $_POST['tahun'];
        							echo "<p>Tanggal: $tanggal</p>";
        							echo "<p>Bulan: $bulan</p>";
       							    echo "<p>Tahun: $tahun</p>";
    								}
    								?>
								</div>	
</div>
			</div>
				</div>
					</div>
						</div>
							</div>
								</div>		
								
								<div class="container-fluid p-0 wow fadeIn" data-wow-delay="0.1s">
			<div id="header-carousel" class="carousel slide" data-bs-ride="carousel bg">
				<div class="carousel-inner">
					<div class="carousel-item active">
						<img class="w-100 h-100" src="<?php base_url() ?>../assets/img/logo/g-rinjani.jpg" alt="Image" />
						<div class="carousel-caption">
							<div class="container">
								<div class="row justify-content-center">
								<div class="bg-success text-center p-3">
								<p> Booking Gunung Kerinci</p>
								<div class="bg-success text-center p-3">
									

</body>
</html>

								</div>	
</div>
			</div>
				</div>
					</div>
						</div>
							</div>
								</div>	
								
										class="btn btn-square btn-outline-primary border-2 m-1"
										href=""
										><i class="fab fa-twitter"></i
									></a>
									<a
										class="btn btn-square btn-outline-primary border-2 m-1"
										href=""
										><i class="fab fa-instagram"></i
									></a>
								</div>
							</div>
							<div class="bg-light text-center p-3">
								<p>Gunung ciremai, gunung tertinggi di jawa barat yang mempunyai ketinggian 3.078mdpl	</p>
								<div class="bg-success text-center p-3">
									<a href="<?php base_url()?>panduan_booking">Lihat Selengkapnya</a>
								</div>
							</div>
						</div>
					</div>
					
					
					
				</div>
			</div>
		</div>
		<!-- Team End -->

# Booking

Bagian booking


# Results

![Screenshot (513)](https://github.com/muhamadfarrasjasir12/e-commers/assets/150880443/e9495a45-75a1-4881-b55e-f96a68aa6580)

![Screenshot (514)](https://github.com/muhamadfarrasjasir12/e-commers/assets/150880443/c80d2dcb-f889-4bd6-8d18-7e896434156b)

![Screenshot (515)](https://github.com/muhamadfarrasjasir12/e-commers/assets/150880443/c6c9be67-c788-48c0-ae8f-f2a9c8ca7318)



