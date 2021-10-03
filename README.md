# Guam's CAR Score (a redux)
## A variation on the original public health metric measuring community spread 

The COVID Area (CAR) Score is a metric designed to provide a single-glance, numerical assessment of a community's level of infection due to the coronavirus pandemic. Created by [Dr. Felix Cabrera](https://www.linkedin.com/in/felix-tudela-cabrera-4b8b937/), the algorithm takes into account (1) incidence of new cases, (2) testing effectiveness, and (3) rate of spread. It's not a [black-box algorithm](https://en.wikipedia.org/wiki/Black_box) - based on a simple algebraic formula, the explainability of each day's generated CAR Score is self-evident. 

It's a computed metric that gauges performance based on data relative to preceding time series - like a Major League pitcher's ERA, not a speculative value like a company's stock price. While it's been seen as a valuable community tool to understanding impact, it's also been misunderstood and misinterpreted. 

![Original CAR Score formula](https://github.com/jasonsalas/guam-car-score-redux/blob/main/CAR_Score_formula.png?raw=true)

The official CAR Score is in its third iteration, modified for newer data inputs and trends. But as the virus evolved, the metric needed to be adjusted in parallel due to the delta variant surge. While still very much applicable, the CAR Score is, in my opinion, due for updating.

Has the CAR Score served its purpose in producing what it was built to? No doubt. Is it repeatable, stable and reliable? You bet. Is it perfect? Certainly not. Could it be made better? The biggest room in the world's the room for self-improvement, baby. 

Because the CAR Score's method is a publicly-available algorithm authored by a local government agency and based on pure objective math, it's implicitly public domain and open source. So I thought I'd take a stab at forking the original formula and revise it to incorporate additional environmental coefficients based on Dr. Cabrera's original concept. I'm putting my own heuristic spin on it and noting any variance in results.

(Also, Felix is a friend and I'm hoping he won't mind me making a couple adjustments for trivial experimentation.)

~~I'm additionally using a time-series database I built using public health data to apply predictive analytics using machine learning.~~
