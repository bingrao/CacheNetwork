

Simulator of experiments presented in "Adaptive Caching Networks with Optimality Guarantees", S. Ioannidis and E. Yeh, SIGMETRICS 2016. Please cite this paper if you intend to use this code for your research.





Command-line arguments
----------------------
Several program parameters can be controlled from the command line.


	usage: CacheNetwork.py [-h] [--max_capacity MAX_CAPACITY]
				       [--min_capacity MIN_CAPACITY] [--max_weight MAX_WEIGHT]
				       [--min_weight MIN_WEIGHT] [--max_rate MAX_RATE]
				       [--min_rate MIN_RATE] [--time TIME] [--warmup WARMUP]
				       [--catalog_size CATALOG_SIZE]
				       [--demand_size DEMAND_SIZE]
				       [--demand_distribution {powerlaw,uniform}]
				       [--powerlaw_exp POWERLAW_EXP]
				       [--query_nodes QUERY_NODES]
				       [--graph_type {erdos_renyi,balanced_tree,hypercube,cicular_ladder,cycle,grid_2d,lollipop,expander,hypercube,star,barabasi_albert,watts_strogatz,regular,powerlaw_tree,small_world,geant,abilene,dtelekom,servicenetwork}]
				       [--graph_size GRAPH_SIZE] [--graph_degree GRAPH_DEGREE]
				       [--graph_p GRAPH_P] [--random_seed RANDOM_SEED]
				       [--debug_level {INFO,DEBUG,WARNING,ERROR}]
				       [--cache_type {LRU,FIFO,LFU,RR,EWMAGRAD,LMIN}]
				       [--query_message_length QUERY_MESSAGE_LENGTH]
				       [--response_message_length RESPONSE_MESSAGE_LENGTH]
				       [--monitoring_rate MONITORING_RATE]
				       [--interpolate INTERPOLATE] [--beta BETA]
				       [--gamma GAMMA] [--expon EXPON] [--T T]
				       outputfile

		Simulate a Network of Caches

		positional arguments:
		  outputfile            Output file

		optional arguments:
		  -h, --help            show this help message and exit
		  --max_capacity MAX_CAPACITY
					Maximum capacity per cache (default: 2)
		  --min_capacity MIN_CAPACITY
					Minimum capacity per cache (default: 2)
		  --max_weight MAX_WEIGHT
					Maximum edge weight (default: 100.0)
		  --min_weight MIN_WEIGHT
					Minimum edge weight (default: 1.0)
		  --max_rate MAX_RATE   Maximum demand rate (default: 1.0)
		  --min_rate MIN_RATE   Minimum demand rate (default: 1.0)
		  --time TIME           Total simulation duration (default: 1000.0)
		  --warmup WARMUP       Warmup time until measurements start (default: 0.0)
		  --catalog_size CATALOG_SIZE
					Catalog size (default: 100)
		  --demand_size DEMAND_SIZE
					Demand size (default: 1000)
		  --demand_distribution {powerlaw,uniform}
					Demand distribution (default: powerlaw)
		  --powerlaw_exp POWERLAW_EXP
					Power law exponent, used in demand distribution
					(default: 1.2)
		  --query_nodes QUERY_NODES
					Number of nodes generating queries (default: 100)
		  --graph_type {erdos_renyi,balanced_tree,hypercube,cicular_ladder,cycle,grid_2d,lollipop,expander,hypercube,star,barabasi_albert,watts_strogatz,regular,powerlaw_tree,small_world,geant,abilene,dtelekom,servicenetwork}
					Graph type (default: erdos_renyi)
		  --graph_size GRAPH_SIZE
					Network size (default: 100)
		  --graph_degree GRAPH_DEGREE
					Degree. Used by balanced_tree, regular,
					barabasi_albert, watts_strogatz (default: 4)
		  --graph_p GRAPH_P     Probability, used in erdos_renyi, watts_strogatz
					(default: 0.1)
		  --random_seed RANDOM_SEED
					Random seed (default: 4156910908)
		  --debug_level {INFO,DEBUG,WARNING,ERROR}
					Debug Level (default: INFO)
		  --cache_type {LRU,FIFO,LFU,RR,EWMAGRAD,LMIN}
					Networked Cache type (default: LRU)
		  --query_message_length QUERY_MESSAGE_LENGTH
					Query message length (default: 0.0)
		  --response_message_length RESPONSE_MESSAGE_LENGTH
					Response message length (default: 0.0)
		  --monitoring_rate MONITORING_RATE
					Monitoring rate (default: 1.0)
		  --interpolate INTERPOLATE
					Interpolate past states, used by LMIN (default: False)
		  --beta BETA           beta used in EWMA (default: 1.0)
		  --gamma GAMMA         gamma used in LMIN (default: 0.1)
		  --expon EXPON         exponent used in LMIN (default: 0.5)
		  --T T                 Suffling period used in LMIN (default: 5.0)
