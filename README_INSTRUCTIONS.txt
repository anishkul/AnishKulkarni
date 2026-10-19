WEBSITE UPDATE 02 — NASA INTERNSHIP BUTTONS + ROCKET CLUB LOGO
===========================================================

BASED ON: Website Update 01 (the previous index.html + portfolio.css).
Only THREE repository files are included in this ZIP:

  index.html                  REPLACE existing file at repository root
  assets/css/portfolio.css    REPLACE existing CSS file
  images/rrc-logo.png         ADD new image

HOW TO APPLY (GitHub website):
1. Open index.html in the root of the GitHub repo. Click Edit (pencil).
   Replace its entire contents with index.html from this ZIP. Commit.
2. Open assets/css/portfolio.css. Click Edit.
   Replace its entire contents with the CSS file from this ZIP. Commit.
3. Navigate to images/, then Add file > Upload files.
   Upload ONLY the new rrc-logo.png image. Commit.
4. Refresh your GitHub Pages website after its deployment completes.

NO OTHER FILES NEED TO BE CHANGED.
The four images from Update 01 stay where they are; don't delete them.

ALTERNATIVE FOR MINIMAL COPY/PASTE:
- In index.html, replace ONLY the NASA card and Ramblin' Rocket Club card.
- In assets/css/portfolio.css, append the NASA topics and rocket logo CSS
  from the bottom of the replacement stylesheet and leave existing CSS.
  The obsolete .rrc-visual styles can be deleted, but are harmless.

COPY/PASTE NASA ARTICLE: Replace the existing article for
"NASA OSTEM Intern / Human Landing System" with the block below:

								<!-- NASA HLS Internship -->
								<article>
									<header>
										<span class="date">August 2026 - December 2026</span>
										<h2>NASA OSTEM Intern<br />Human Landing System</h2>
									</header>
									<div class="experience-media experience-media--logo experience-media--nasa">
										<img src="images/nasa-logo.png" alt="NASA insignia" loading="lazy" decoding="async" />
									</div>
									<p>At NASA Marshall Space Flight Center, I'm contributing to lunar Terrain Relative Navigation (TRN) simulation for the Human Landing System. My work focuses on realistic camera imagery, lunar terrain and lighting models, and simulation workflows that support guidance and navigation testing.</p>

									<!-- Accessible click-to-expand project and skills buttons. No JavaScript required. -->
									<h3 class="nasa-topics-heading">Projects &amp; Technical Skills</h3>
									<p class="nasa-topics-intro">Explore my current technical focus areas:</p>
									<div class="nasa-topics">
										<details class="nasa-topic">
											<summary>Simulation Integration</summary>
											<div class="nasa-topic-content">
												<p>Integrating Unreal Engine imagery with a six-degree-of-freedom (6-DoF) guidance, navigation, and control simulation. This work involves co-simulation, debugging, image-quality checks, and verification of simulation behavior.</p>
											</div>
										</details>

										<details class="nasa-topic">
											<summary>Lunar Terrain &amp; Lighting</summary>
											<div class="nasa-topic-content">
												<p>Working with lunar digital elevation models (DEMs) and albedo data to improve simulated terrain and surface reflectance. Key skills include terrain visualization, material and lighting workflows, and validation of rendered scenes.</p>
											</div>
										</details>

										<details class="nasa-topic">
											<summary>Camera &amp; Image Modeling</summary>
											<div class="nasa-topic-content">
												<p>Developing higher-fidelity synthetic camera imagery by accounting for general optical effects such as lens distortion. My focus includes camera modeling, image verification, and identifying differences between idealized and more realistic imagery.</p>
											</div>
										</details>

										<details class="nasa-topic">
											<summary>Simulation &amp; Monte Carlo Testing</summary>
											<div class="nasa-topic-content">
												<p>Supporting Linux-based and parallel simulation workflows to make navigation testing more scalable and repeatable. This involves cross-platform development, troubleshooting, and Monte Carlo simulation concepts for evaluating system behavior.</p>
											</div>
										</details>

										<details class="nasa-topic nasa-topic--skills">
											<summary>Tools &amp; Skills</summary>
											<div class="nasa-topic-content">
												<ul class="nasa-skill-list">
													<li>Unreal Engine</li>
													<li>6-DoF / GNC Simulation</li>
													<li>MATLAB / Simulink</li>
													<li>Linux</li>
													<li>Lunar DEMs &amp; Albedo</li>
													<li>Camera Modeling</li>
													<li>Debugging &amp; Verification</li>
													<li>Monte Carlo Methods</li>
												</ul>
											</div>
										</details>
									</div>
								</article>

COPY/PASTE RAMBLIN' ROCKET CLUB ARTICLE: Replace the existing
"Guidance, Navigation & Control / Ramblin' Rocket Club" card with:

								<!-- Ramblin' Rocket Club -->
								<article>
									<header>
										<span class="date">August 2025 - December 2025</span>
										<h2>Guidance, Navigation &amp; Control<br />Ramblin' Rocket Club</h2>
									</header>
									<div class="experience-media experience-media--logo experience-media--rrc-logo">
										<img src="images/rrc-logo.png" alt="Georgia Tech Ramblin' Rocket Club logo" loading="lazy" decoding="async" />
									</div>
									<p>Updated GNCSIM with a calibrated actuator model and validated closed-loop response against static-fire data. Implemented actuator modeling in flight software with deflection and rate limits, verifying hardware-in-the-loop and software-in-the-loop command tracking.</p>
								</article>

COPY/PASTE ADDITIONAL CSS:
(Append this to the bottom of assets/css/portfolio.css if editing manually.)

/* Ramblin' Rocket Club logo: keep its original proportions and clean background. */
#main > .posts .experience-media--rrc-logo {
  background: #fff;
  padding: 0.65rem;
}

/* Clickable NASA project/skills buttons; native details elements work without JS. */
#main > .posts .nasa-topics-heading {
  font-size: 0.95rem;
  line-height: 1.4;
  letter-spacing: 0.065em;
  margin: 1.75rem 0 0.25rem;
}

#main > .posts p.nasa-topics-intro {
  margin: 0 0 1rem;
  text-align: center;
  font-size: 0.9rem;
}

#main > .posts .nasa-topics {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 0.65rem;
  text-align: left;
}

#main > .posts .nasa-topic {
  min-width: 0;
  margin: 0;
  border: 1px solid #c4ceda;
  border-radius: 0.3rem;
  background: #f8fafc;
}

#main > .posts .nasa-topic--skills {
  grid-column: 1 / -1;
}

#main > .posts .nasa-topic > summary {
  list-style: none;
  position: relative;
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 0.5rem;
  width: 100%;
  min-height: 3.1rem;
  padding: 0.75rem 0.85rem;
  cursor: pointer;
  font: 700 0.65rem/1.5 "Source Sans Pro", Helvetica, sans-serif;
  letter-spacing: 0.025em;
  text-transform: uppercase;
  color: #153857;
  transition: background 0.2s ease;
}

#main > .posts .nasa-topic > summary::-webkit-details-marker {
  display: none;
}

#main > .posts .nasa-topic > summary::after {
  content: "+";
  flex: 0 0 auto;
  font-size: 1.15rem;
  font-weight: 400;
  line-height: 1;
}

#main > .posts .nasa-topic[open] > summary::after {
  content: "−";
}

#main > .posts .nasa-topic > summary:hover,
#main > .posts .nasa-topic[open] > summary {
  background: #e9f1f7;
}

#main > .posts .nasa-topic > summary:focus-visible {
  outline: 3px solid #2489bf;
  outline-offset: 2px;
}

#main > .posts .nasa-topic-content {
  padding: 0.8rem 0.85rem 0.95rem;
  border-top: 1px solid #d7e0e8;
}

#main > .posts .nasa-topic-content p {
  margin: 0;
  font-size: 0.85rem;
  line-height: 1.65;
  text-align: left;
  overflow-wrap: anywhere;
}

#main > .posts .nasa-skill-list {
  display: flex;
  flex-wrap: wrap;
  gap: 0.4rem;
  margin: 0;
  padding: 0;
  list-style: none;
}

#main > .posts .nasa-skill-list li {
  margin: 0;
  padding: 0.3rem 0.55rem;
  background: #e5edf4;
  border-radius: 999px;
  color: #163d5a;
  font-size: 0.73rem;
  line-height: 1.4;
}

@media screen and (max-width: 480px) {
  #main > .posts .nasa-topics {
    grid-template-columns: 1fr;
  }
  #main > .posts .nasa-topic--skills {
    grid-column: auto;
  }
}


PUBLIC PORTFOLIO CAUTION:
The experience copy deliberately avoids naming partner-specific algorithms,
nonpublic simulation architectures, sensor specifications, calibration data,
benchmarks, or internal documents. Since this is a preliminary project plan,
the portfolio uses ongoing-work wording rather than completed-result claims.
Seek approval from your NASA supervisor/public affairs contact before publishing
technical details about your internship work, especially partner-linked work.
