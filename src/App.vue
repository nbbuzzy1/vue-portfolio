<template>
  <div id="app">
	<!-- Sidebar -->
			<section id="sidebar">
				<div class="inner">
					<nav>
						<ul>
							<li><a href="#intro">Welcome</a></li>
							<li><a href="#one">Projects</a></li>
							<li><a href="#two">Skills</a></li>
							<li><a href="#three">Get in touch</a></li>
						</ul>
					</nav>
				</div>
			</section>
		<!-- Wrapper -->
			<div id="wrapper">

				<!-- Intro -->
					<section id="intro" class="wrapper style1 fullscreen fade-up">
						<div class="inner">
							<h1>Nicholas Buzzy, J.D.</h1>
							<p>Software developer and lawyer, but I am always an entrepreneur at heart.</p>
							<ul class="actions">
								<li><a href="#one" class="button scrolly">Learn more</a></li>
							</ul>
						</div>
					</section>

				<!-- Projects -->
					<section id="one" class="wrapper style2 spotlights">
						<section id="project-one">
							<div class="content">
								<div class="inner">
									<h2>BuzzyCite</h2>
									<p>Founder and CEO.  Created the largest free search engine for court cases.  Developed algorithm that correctly cites court cases.  Built with MEAN stack.  </p>
									<ul class="actions">
										<li><a href="https://buzzycite.com" target="_blank" class="button">Learn more</a></li>
									</ul>
								</div>
							</div>
						</section>
						<section id="project-two">
							<div class="content">
								<div class="inner">
									<h2>Buzzy Price</h2>
									<p>Founder and CEO.  Built the ultimate eBay price tracker where we allow users to set custom alerts for price updates.</p>
									<ul class="actions">
										<li><a href="https://buzzyprice.com" class="button">Learn more</a></li>
									</ul>
								</div>
							</div>
						</section>
					</section>
				<!-- Skills -->
					<section id="two" class="wrapper style3 fade-up">
						<div class="inner">
							<h2>Skills</h2>
							<p>Phasellus convallis elit id ullamcorper pulvinar. Duis aliquam turpis mauris, eu ultricies erat malesuada quis. Aliquam dapibus, lacus eget hendrerit bibendum, urna est aliquam sem, sit amet imperdiet est velit quis lorem.</p>
							<div class="features">
								<section>
									<span class="icon solid major fa-code"></span>
									<h3>Lorem ipsum amet</h3>
									<p>Phasellus convallis elit id ullam corper amet et pulvinar. Duis aliquam turpis mauris, sed ultricies erat dapibus.</p>
								</section>
								<section>
									<span class="icon solid major fa-lock"></span>
									<h3>Aliquam sed nullam</h3>
									<p>Phasellus convallis elit id ullam corper amet et pulvinar. Duis aliquam turpis mauris, sed ultricies erat dapibus.</p>
								</section>
								<section>
									<span class="icon solid major fa-cog"></span>
									<h3>Sed erat ullam corper</h3>
									<p>Phasellus convallis elit id ullam corper amet et pulvinar. Duis aliquam turpis mauris, sed ultricies erat dapibus.</p>
								</section>
								<section>
									<span class="icon solid major fa-desktop"></span>
									<h3>Veroeros quis lorem</h3>
									<p>Phasellus convallis elit id ullam corper amet et pulvinar. Duis aliquam turpis mauris, sed ultricies erat dapibus.</p>
								</section>
								<section>
									<span class="icon solid major fa-link"></span>
									<h3>Urna quis bibendum</h3>
									<p>Phasellus convallis elit id ullam corper amet et pulvinar. Duis aliquam turpis mauris, sed ultricies erat dapibus.</p>
								</section>
								<section>
									<span class="icon major fa-gem"></span>
									<h3>Aliquam urna dapibus</h3>
									<p>Phasellus convallis elit id ullam corper amet et pulvinar. Duis aliquam turpis mauris, sed ultricies erat dapibus.</p>
								</section>
							</div>
						</div>
					</section>
				<!-- Get in Touch -->
					<section id="three" class="wrapper style1 fade-up">
						<div class="inner">
							<h2>Get in touch</h2>
							<!-- <p>.</p> -->
							<div class="split style1">
								<section>
									<form method="post" action="#">
										<div class="fields">
											<div class="field half">
												<label for="name">Name</label>
												<input type="text" name="name" id="name" />
											</div>
											<div class="field half">
												<label for="email">Email</label>
												<input type="text" name="email" id="email" />
											</div>
											<div class="field">
												<label for="message">Message</label>
												<textarea name="message" id="message" rows="5"></textarea>
											</div>
										</div>
										<ul class="actions">
											<li><a href="" class="button submit">Send Message</a></li>
										</ul>
									</form>
								</section>
								<section>
									<ul class="contact">
										<li>
											<h3>Social</h3>
											<ul class="icons">
												<li><a href="#" class="icon brands fa-github"><span class="label">GitHub</span></a></li>
												<li><a href="#" class="icon brands fa-linkedin-in"><span class="label">LinkedIn</span></a></li>
												<li><a href="#" class="icon brands fa-facebook-f"><span class="label">Facebook</span></a></li>
											</ul>
										</li>
									</ul>
								</section>
							</div>
						</div>
					</section>
			</div>
  </div>
</template>

<script>
export default {
  name: 'App',
}
</script>

<style>
.wrapper.style1 {
    background-color: #116466;
}

#sidebar {
    background: #2C3531;
}

#sidebar nav a {
	color: #D1E8E2;
	/* border-bottom: 1px solid #D1E8E2; */
}

@media(min-width: 1280px) {
	#sidebar nav a {
		border-bottom: 1px solid #D1E8E2;
	}
}

#project-one {
	background: #ffcb9a;
	color: #2C3531;
}

#project-one h2, #project-two h2, #project-one a.button, #project-two a.button {
	color: #2C3531 !important;
}

#project-one a.button, #project-two a.button {
	color: #2C3531 !important;
	border-color: #2C3531 !important;
}

#project-two {
	background: #d9b08c;
	color: #2C3531;
}

.wrapper.style3 {
	background: #d1e8e2;
	color: #2c3531;
}

.wrapper.style3 h2, .wrapper.style3 h3, .wrapper.style3 .icon, .wrapper.style3 .icon.major:before {
	color: #2c3531 !important;
}
</style>
