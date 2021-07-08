<template>
  <div id="app">
	<!-- Sidebar -->
			<section id="sidebar">
				<div class="inner">
					<nav>
						<ul>
							<li><a href="#intro">Welcome</a></li>
							<li><a href="#projects">Projects</a></li>
							<li><a href="#skills">Skills</a></li>
							<li><a href="#contact">Get in touch</a></li>
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
							<p>Experienced senior software developer.  Former litigator.  Always an entrepreneur.</p>
							<ul class="actions">
								<li><a href="#projects" class="button scrolly">Learn more</a></li>
							</ul>
						</div>
					</section>

				<!-- Projects -->
					<section id="projects" class="wrapper style2 spotlights">
						<section id="project-one">
							<a href="https://buzzycite.com" target="_blank" class="image"><img src="../public/assets/images/buzzycite.jpg" alt="" data-position="center center" /></a>
							<div class="content">
								<div class="inner">
									<h2>BuzzyCite</h2>
									<p>Founder and CEO.  Created the largest free search engine for court cases.  Developed algorithm that correctly cites court cases.  
										Featured by 
										<a	class="buzzycite-media-link"
											target="_blank"
											href="https://case.law/gallery/applications-third-party"
										>
											Harvard Law School</a> and 
										<a	class="buzzycite-media-link" 
											target="_blank"
											href="https://www.lawsitesblog.com/2020/06/new-legal-research-tool-taps-into-caselaw-access-projects-6-7m-cases.html"
										>
											LawSites</a>.
									</p>
									<ul class="actions">
										<li><a href="https://buzzycite.com" target="_blank" class="button">See BuzzyCite</a></li>
									</ul>
								</div>
							</div>
						</section>
						<section id="project-two">
							<a href="https://buzzyprice.com" target="_blank" class="image"><img src="../public/assets/images/buzzyprice.jpg" alt="" data-position="top center" /></a>
							<div class="content">
								<div class="inner">
									<h2>Buzzy Price</h2>
									<p>Founder and CEO.  Developed an eBay price tracker that allows users to set custom alerts for price updates on auction items.</p>
									<ul class="actions">
										<li><a href="https://buzzyprice.com" target="_blank" class="button">See Buzzy Price</a></li>
									</ul>
								</div>
							</div>
						</section>
					</section>
				<!-- Skills -->
					<section id="skills" class="wrapper style3 fade-up">
						<div class="inner">
							<h2>Skills</h2>
							<p>Below are the most frequently used technical skills. Additional skills include those gained from six years litigation experience (including thirteen jury trials) and serving as the founder and CEO of two startup businesses.</p>
							<div class="features">
								<section>
									<span class="icon solid major"><i class="fab fa-angular"></i></span>
									<h3>Angular</h3>
									<p>Use for enterprise applications such as BuzzyCite and implement its observables, dependency injection, and TypeScript models.</p>
								</section>
								<section>
									<span class="icon solid major"><i class="fab fa-vuejs"></i></span>
									<h3>Vue.js</h3>
									<p>Lightweight front end framework used with Buzzy Price and this portfolio page.  State management with Vuex.</p>
								</section>
								<section>
									<span class="icon solid major"><i class="fab fa-node"></i></span>
									<h3>Node.js</h3>
									<p>Implement this server technoology with BuzzyCite and Buzzy Price.  Express framework for API route management and database connections.</p>
								</section>
								<section>
									<span class="icon solid major"><i class="fab fa-python"></i></span>
									<h3>Python</h3>
									<p>Automation, data science, and web scraping for various applications.  Flask framework for building APIs.</p>
								</section>
								<section>
									<span class="icon solid major fa-database"></span>
									<h3>MongoDB</h3>
									<p>Database for BuzzyCite.  Manage users and citation data.  Enforce authentication and usage limits.</p>
								</section>
								<section>
									<span class="icon solid major"><i class="fab fa-css3"></i></span>
									<h3>HTML5/CSS3</h3>
									<p>Extensive use with every project.  Additionally, utilize SCSS for BuzzyCite and SASS with Buzzy Price.</p>
								</section>
							</div>
						</div>
					</section>
				<!-- Get in Touch -->
					<section id="contact" class="wrapper style1 fade-up">
						<div class="inner">
							<h2>Get in touch</h2>
							<!-- <p>.</p> -->
							<div class="split style1">
								<section>
									<form method="post" action="#" v-on:submit.prevent>
										<div class="fields">
											<div class="field half">
												<label for="name">Name</label>
												<input type="text" name="name" id="name" v-model="name" maxlength="75" required />
											</div>
											<div class="field half">
												<label for="email">Email</label>
												<input type="email" name="email" id="email" v-model="email" maxlength="75" required />
											</div>
											<div class="field">
												<label for="message">Message</label>
												<textarea name="message" id="message" rows="5" v-model="message" style="resize: none;" maxlength="5000" required></textarea>
											</div>
										</div>
										<ul class="actions">
											<li><a class="button submit" @click="sendMessage">Send Message</a></li>
										</ul>
										<div v-if="errors.length">
											<div v-for="error of errors" v-bind:key="error" class="error">{{ error }}</div>
										</div>
										<div v-if="showSuccess" class="success-msg">Message successfully sent!</div>
									</form>
								</section>
								<section>
									<ul class="contact">
										<li>
											<h3 class="social">Social</h3>
											<ul class="icons">
												<li><a href="https://www.linkedin.com/in/nicholas-buzzy/" target="_blank" class="icon brands fa-linkedin-in"><span class="label">LinkedIn</span></a></li>
												<li><a href="https://github.com/nbbuzzy1" target="_blank" class="icon brands fa-github"><span class="label">GitHub</span></a></li>
												<li><a href="https://www.facebook.com/nbbuzzy23" target="_blank" class="icon brands fa-facebook-f"><span class="label">Facebook</span></a></li>
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
import axios from 'axios'
export default {
  name: 'App',
  data() {
	return {
		url: process.env.VUE_APP_URL,
		email: '',
		name: '',
		message: '',
		errors: [],
		showSuccess: false
	}
  },
  methods: {
	async sendMessage() {
		this.showSuccess = false;
		this.errors = [];

		if (this.email && this.name && this.message) {
			const params = { userEmail: this.email.trim(), name: this.name.trim(), message: this.message.trim() }
			
			try {
				const result = await axios.post(`${this.url}/contact-me`, params);
				
				if (result) {
					this.showSuccess = true;
					this.email = '';
					this.name = '';
					this.message = '';
					setTimeout(() => this.showSuccess = false, 3000)
				}
			} catch {
				this.email = '';
				this.name = '';
				this.message = '';
			}
		} else {
			if (!this.email) {
				this.errors.push('Please include an email.')
			}
			if (!this.name) {
				this.errors.push('Please include your name.')
			}
			if (!this.message) {
				this.errors.push('Please include a message.')
			}
		}
	}
  }
}
</script>

<style>

html {
	scroll-behavior: smooth
}

body {
	background: #D1E8E2 !important;
}

input, textarea, .error, .success-msg {
	color: white !important;
}

.buzzycite-media-link {
	border-bottom-color: black;
}

.wrapper.style1 {
    background-color: #116466;
}

#sidebar {
    background: #2C3531;
}

#sidebar nav a {
	color: #D1E8E2;
}

#project-one {
	background: #ffcb9a;
	color: #2C3531;
}

.spotlights > #project-one > .image:before {
		background: #ffcb9a !important;
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

.spotlights > #project-two > .image:before {
	background: #d9b08c !important;
}

#project-one img, #project-two img {
	display: block;
    max-width: 100%;
    max-height: 450px;
    width: auto;
    height: auto;
}

#project-one .image, #project-two .image {
	display: flex;
    align-items: center;
}

.wrapper.style3 {
	background: #d1e8e2;
	color: #2c3531;
}

.wrapper.style3 h2, .wrapper.style3 h3, .wrapper.style3 .icon, .wrapper.style3 .icon.major:before {
	color: #2c3531 !important;
}

.contact .icons .icon {
	font-size: 30px;
	margin-right: 10px;
}

@media(min-width: 1280px) {
	#sidebar nav a {
		border-bottom: 1px solid #D1E8E2 !important;
	}
}

@media(max-width: 980px) {
	#project-one img, #project-two img {
		max-width: 100%;
		max-height: 100%;
		margin-top: 50px;
	}

	#project-one .image, #project-two .image {
		justify-content: center;
	}
}
</style>
