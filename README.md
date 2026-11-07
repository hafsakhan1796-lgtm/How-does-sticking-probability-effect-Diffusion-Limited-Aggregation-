# How-does-sticking-probability-effect-the-structure of a DLA cluster?
# Overview 
Diffusion-limited aggregation (DLA) is a computational model that represents noisy growth that is limited by diffusion in a random environment.  The idea behind the mechanism is a simple one. You start with a random nucleation center, with a single particle of a certain radius, let’s say R, placed at the center. This is followed by the release of a second particle at a random point some distance away. The newly released particle is allowed to diffuse in a random direction until it happens to be within a radius R of the first particle. At the point of contact, the second particle is allowed to aggregate with the first particle in the center. Then a second walker (a different name for a particle) is added at a random position and allowed to diffuse until it is within the radius of either the first walker or the second, and it is allowed to aggregate, and so on. A DLA cluster is then formed because of the addition of N-1 particles to the particle at the center. 


For this project, I used Python to explore how the sticking probability of a particle effect a DLA cluster. 


I used three different sticking probabilities: 


  - **1.0 - 100% sticking probability:** every particle that comes close to the cluster sticks. 

  - **0.5 - 50% sticking probability:** a particle has 50% chance of sticking once it comes closer to the cluster. 

  - **0.1- 10% sticking probability:** a particle has 10% chance of sticking once it comes closer to the cluster. 

By comparing the resulting cluster, I wanted to understand how sticking probability effects the cluster growth, branching patterns and the overall morphology. 

## Research Question 

How does sticking probability influence the growth and structure of a DLA cluster? 

## Scientific Background 

# What is Diffusion-Limited Aggregation? 

Diffusion-limited aggregation (DLA) is a computational model that represents noisy growth that is limited by diffusion in a random environment.  The idea behind the mechanism is a simple one. You start with a random nucleation center, with a single particle of a certain radius, let’s say R, placed at the center. This is followed by the release of a second particle at a random point some distance away. The newly released particle is allowed to diffuse in a random direction until it happens to be within a radius R of the first particle. At the point of contact, the second particle is allowed to aggregate with the first particle in the center. Then a second walker (a different name for a particle) is added at a random position and allowed to diffuse until it is within the radius of either the first walker or the second, and it is allowed to aggregate, and so on. A DLA cluster is then formed because of the addition of N-1 particles to the particle at the center. 

## Why do DLA Clusters Form Branches? 

One important explanation is **screening.** The idea is as follows: when a new particle is allowed to diffuse, it walks a certain distance and gets captured by another particle; do this often enough, and you get a nice branch that keeps capturing new oncoming particles. Because the branches keep “capturing” the new particles before they can diffuse deep inside, the spaces or the “Fjords” do not get filled up. Thus, we say, “the fjords are screened.” 
In his article, Sanders states that “The larger-scale structure of a DLA cluster is dominated by non-local effects.” A non-local effect, simply put, refers to the idea that something happening at one point can influence the behavior of something else happening at a different point. In the context of the DLA clusters, non-local effects are governed by screening. An incoming particle is captured by a branch and fails to reach a different area; thus, the branch that captures the particles early keeps growing while other parts of the clusters remain small. Therefore, the shape of a DLA cluster is influenced by where the next particle will attach, causing larger branches in a particular area and shorter branches elsewhere, as well as leaving the ‘fjords” unfilled. 

## What Causes the Clusters to Become Rough? 

Starting with a smooth surface does not necessarily mean the resulting cluster will be smooth. In DLA, the formation of bumps on the surface is due to **shot noise** in the arrival of the particle. Shot noise is the random fluctuations in the arrival of particles. Because of screening and shot noise, a smooth surface can lead to bumps and a rougher surface, yielding a rough cluster. How do these bumps form? They can grow because of instability, which is followed by tip-splitting. Tip splitting happens due to screening, where some growing branches can split into tips due to random fluctuations; thus, repeated splitting, growing, and branching can give rise to fractals (structures with patterns and complexity that can appear across different length scales).





