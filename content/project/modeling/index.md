---
title: Computational Modeling
summary: Demonstrating the use of computers to simulate and study complex systems using mathematics, physics and computer science.
tags:
- Computational Modeling
- Modeling
- Thermal Models
- 2D Models
- 3D Models
- Geothermal Models
date: "2016-04-27T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

# image:
#   caption: Photo by rawpixel on Unsplash
#   focal_point: Smart

links:
# - icon: twitter
#   icon_pack: fab
#   name: Follow
#   url: https://twitter.com/georgecushen
url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
# slides: example
---

Computational modeling is the use of computers to simulate and study complex systems using mathematics, physics and computer science. A computational model contains numerous variables that characterize the system being studied. Rather than deriving a mathematical analytical solution to the problem, experimentation with the model is done by adjusting the parameters of the system in the computer, and studying the differences in the outcome of the experiments. Simulation is done by adjusting the variables alone or in combination and observing the outcomes.

I conduct computational modeling with a program written in C++ called Finite Difference Heat Flow Simulation (or ARC, for short), which is a type of finite element analysis (or FEM).  ARC was developed in order to perform finite difference determination of steady-state heat flow by calculating temperature and heat generation for a given system subdivided into cells and heat transfer to and from surrounding cells.  In order to perform the analysis, a system is modeled using ASCII format input codes and desired values of system parameters in a Microsoft Excel file:  thermal conductivity, radiogenic heat production, basal heat flow, heat capacity of rock and fluid density, advection constraints, starting temperatures, velocity, and direction and cell size and model dimensions.
