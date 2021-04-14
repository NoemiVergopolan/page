---

title: "HPC simulations of brownout: A noninteracting particles dynamic model"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- Roberto Porcù
- Edie Miglio
- Nicola Parolini
- Mattia Penati
- admin

# Author notes (optional)
author_notes:
- ""
- ""

# Paper publication date
date: "2020-02-17T00:00:00Z"
doi: "10.1177/1094342020905971"

# Schedule webpage page publish date (NOT publication's date).
publishDate: ""

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: In *International Journal of High Performance Computing Applications*
publication_short:  

abstract: Helicopters can experience brownout when flying close to a dusty surface. The uplifting of dust in the air can remarkably restrict the pilot’s visibility area. Consequently, a brownout can disorient the pilot and lead to the helicopter collision against the ground. Given its risks, brownout has become a high-priority problem for civil and military operations. Proper helicopter design is thus critical, as it has a strong influence over the shape and density of the cloud of dust that forms when brownout occurs. A way forward to improve aircraft design against brownout is the use of particle simulations. For simulations to be accurate and comparable to the real phenomenon, billions of particles are required. However, using a large number of particles, serial simulations can be slow and too computationally expensive to be performed. In this work, we investigate an message passing interface (MPI) + graphics processing unit (multi-GPU) approach to simulate brownout. In specific, we use a semi-implicit Euler method to consider the particle dynamics in a Lagrangian way, and we adopt a precomputed aerodynamic field. Here, we do not include particle–particle collisions in the model; this allows for independent trajectories and effective model parallelization. To support our methodology, we provide a speedup analysis of the parallelization concerning the serial and pure-MPI simulations. The results show (i) very high speedups of the MPI + multi-GPU implementation with respect to the serial and pure-MPI ones, (ii) excellent weak and strong scalability properties of the implemented time-integration algorithm, and (iii) the possibility to run realistic simulations of brownout with billions of particles at a relatively small computational cost. This work paves the way toward more realistic brownout simulations, and it highlights the potential of high-performance computing for aiding and advancing aircraft design for brownout mitigation.

# Summary. An optional shortened abstract.
summary:

tags: [HPC, GPU, CUDA, MPI, Particle Dynamics]

# Display this page in the Featured widget?
featured: false

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: https://www.researchgate.net/profile/Roberto-Porcu/publication/339317777_HPC_simulations_of_brownout_A_noninteracting_particles_dynamic_model/links/5e8fed26299bf130798da8f9/HPC-simulations-of-brownout-A-noninteracting-particles-dynamic-model.pdf
url_code: ''
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: 'Illustrations of the analytical air velocity'
  focal_point: ''
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects: 
#- example

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: #example

---

