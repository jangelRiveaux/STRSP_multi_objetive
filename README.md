# STRSP_multi_objetive

This repository contains all instances and results of the tests presented in the subscribed paper "Scheduling technicians and tasks through a multi-objective Biased Random-Key Genetic Algorithm" by th eauthors R. B. Damm,  J. A. R. Merino, A. Chaves and D. P. Ronconi. The repository is stuctured as follows:
```bash
.    
├── Instancias    		
├── README.md	    	
└── Resultados	    	
    ├── BRKGA-QL    		
    ├── NSGA-II	    	
    └── SPEA2	  
 ```

Folder "Instancias" contains all the instances used for testing. Each file ".txt" represent an instance.  Folder "Resultados" contains te result of each algorithm tested in each subfolder "BRKGA-QL", "NSGA-II" and "SPEA2". 



# Instances 

The generated instances are based on the reference instances of Solomon (1987) for the vehicle routing problem with time windows. The following parameters were varied: i ) length of tasks’ time windows, ii ) type of geographical distribution, and iii ) number of tasks and technicians as follows. Time windows were classified into three different scenarios, namely, short, long, and random; a short time window [e, ℓ] corresponding to ℓ−e ∈ {1.5h, 2h, . . . , 3.5h}, a long time window corresponding to ℓ − e ∈ {6.5h, 7h, . . . , 9h}, and a random time window corresponding to ℓ − e ∈ \{1.5h, 2h, . . . , 9h\}. Geographical distributions were classified as (R) random uniform distribution, (C) clustered distribution, and (RC) semi-clustered distribution as suggested in Solomon (1987). There were considered eleven combinations of a number of tasks and technicians as depicted in Table 1, totaling 99 = 3 × 3 × 11 instances. (The last column of Table 1 will be further described in Section ??.)????
 
  
Case | #tasks (n) | #tech. (m) | time limit  
--- | --- | ---| ---
 1  | 16  |  2 |   10  
 2  | 26  |  2 |   20  
 3  | 30  |  3 |   30  
 4  | 39  |  3 |   60 
 5  | 80  | 13 |  240  
 6  | 100 | 10 |  300  
 7  | 100 | 15 |  360  
 8  | 150 | 15 |  600  
 9  | 150 | 25 |  900  
 10 | 200 | 20 | 1200  
 11 | 200 | 30 | 1800  

 

 
 The name of each instance file is STRSP_<type of geographical distribution>_ xxxxx . Each instance file is structured as:
 
 \<number of task\> 
 
 \<number of technician\>


...
 
 
 
# Results 
 




