# CI2024_lab2
Lab 2 of computational intelligence



The best performer is lab2Nuovo, you can run to get good results the code with a popoulation of 200 and 20_000 generations
you will get good (usually optimal) results (not in china ofc) in reasonable time

if you have time to spare i got china down to 54877.11 km (in 3,5 hours mind you) with a population of 400 and 20_000 generations, and it was still improving...


Lab2 is the one where i was experimenting with new stuff, but has become really slow with the progressive updates...
I do not suggest you run it, but if you have a couple hours to spare you are more than welcome to do XD.



The algorithm leverages a Genetic Algorithm (GA) to approximate the shortest path. Key components include:

Population Initialization: The population consists of a mix of routes:
  Greedy routes starting from various cities to create reasonable initial paths.
  Random routes for diversity.
  
Fitness Evaluation: Routes are evaluated by their total distance. The fitness score is inversely proportional to the route's distance, incentivizing shorter paths.

Selection: Uses roulette wheel selection to probabilistically favor shorter routes for breeding.

Crossover (PMX): Implements Partially Mapped Crossover (PMX) to produce valid children that inherit features from both parents without creating duplicates, thus preserving city visitation requirements.

Mutation: Applies two mutation strategies:
  Inversion Mutation: Randomly reverses a segment within a route to explore alternative subpaths.
  Insertion Mutation: Randomly repositions a city within a route, providing further diversity and exploring additional neighborhood routes.

Elitism: Preserves a portion of the top-performing routes in each generation to retain good solutions across generations.





In the code i have a couple of mutate algorithms, the one uncommented right now is the best performer one, if you want you can also try the other ones, they all work, albeit a bit slower.
