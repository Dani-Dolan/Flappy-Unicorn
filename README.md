# Flappy-Unicorn :unicorn:
Visit https://flappy-unicorn.github.io/ to see it in Action!

![Screenshot](unicornvid.gif)

## Neuroevolution and Genetic Algorithms 
Trained an agent to play effectively in a simulation of a simple game. The agent's neural network evolves overtime making it better at the game. 

## Synaptic Library
https://github.com/cazala/synaptic

## Q Learning
The purpose of Q-Learning is to learn a policy, which tells an agent what action to take under what circumstances. It does not require a model of the environment and can handle problems with several changes, as long as it has rewards.
NeuroEvolution Library
Use:
```
// Initialize 
var ne = new Neuroevolution ({options}); 

// Default options values 
var options = { 
    network: [1, [1], 1], // Perceptron structure 
    population: 50, // Population by generation 
    elitism: 0.2, // Best networks kepts unchanged for the next generation (rate ) 
    randomBehavior: 0.2, // New random networks for the next generation (rate) 
    mutationRate: 0.1, // Mutation rate on the weights of synapses 
    mutationRange: 0.5, // Interval of the mutation changes on the synapse weight 
    historic: 0, / / Latest generations saved 
    lowHistoric: false, // Only save score (not the network)
    scoreSort: -1, // Sort order (-1 = desc, 1 = asc) 
    nbChild: 1 // number of child by breeding 
} 


// Update options at any time 
ne.set ({options}); 

// Generate first or next generation 
var generation = ne.nextGeneration (); 

// When an network is over -> save this score 
ne.networkScore (generation [x], <score = 0>);
```
