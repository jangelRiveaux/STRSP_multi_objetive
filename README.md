# STRSP_multi_objetive

This repository contains all instances and results of the tests presented in the subscribed paper "Scheduling technicians and tasks through a multi-objective Biased Random-Key Genetic Algorithm" by th eauthors R. B. Damm,  J. A. R. Merino, A. Chaves and D. P. Ronconi. The repository is stuctured as follows:
```bash
.    
├── Instances    		
├── README.md	
├── STRSP_C_2_2.txt
├── BRKGA-QL - grafic exemple.xlsx	
└── Results    	
    ├── BRKGA-QL    		
    ├── NSGA-II	    	
    └── SPEA2	  
 ```

Folder "Instances" contains all the instances used for testing. Each file ".txt" represent an instance.  Folder "Results" contains te result of each algorithm tested in each subfolder "BRKGA-QL", "NSGA-II" and "SPEA2". "STRSP_C_2_2.txt" is the example instance used in the paper and "BRKGA-QL - grafic exemple.xlsx"	 contain the result obtained for this example.



# Instances 

The generated instances are based on the reference instances of Solomon (1987) for the vehicle routing problem with time windows. The following parameters were varied: i ) length of tasks’ time windows, ii ) type of geographical distribution, and iii ) number of tasks and technicians as follows. Time windows were classified into three different scenarios, namely, short, long, and random; a short time window [e, ℓ] corresponding to ℓ−e ∈ {1.5h, 2h, . . . , 3.5h}, a long time window corresponding to ℓ − e ∈ {6.5h, 7h, . . . , 9h}, and a random time window corresponding to ℓ − e ∈ \{1.5h, 2h, . . . , 9h\}. Geographical distributions were classified as (R) random uniform distribution, (C) clustered distribution, and (RC) semi-clustered distribution as suggested in Solomon (1987). There were considered eleven combinations of a number of tasks and technicians as depicted in Table 1, totaling 99 = 3 × 3 × 11 instances. 


  
  
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
 

 
 The name of each instance file is STRSP_<type of geographical distribution>_<case ID number>_<number Id of instance>; where the geographical distribution can be R, C or RC, the case ID number can be 1 to 11, and the number ID of the instance is 1 if the time window is small, 2 is time window is large and 3 if the time window is randomly created. Each instance file is structured as:
 
 \<number of task\> 
 
 \<number of technician\>
 
 \<task 0 priority = 0\>
 
 \<task 1 priority\>
 
 ...
 
 \<task n priority\>
 
 \<lunch of tecnician 1 priority as top priority\>
 
 \<lunch of tecnician 2 priority as top priority\>
 
 ...
 
 \<lunch of tecnician m priority as top priority\>
 
 
 
 \<tecnician 1 habilities for each task \>
 
 \<tecnician 2 habilities for each task \>
 
 ...
 
 \<tecnician m habilities for each task \>
 
 
 
 \<processing time from tasks from 0 to n\>
 
 \<start of the time windows from tasks from 0 to n\>
 
 \<end of the time windows from tasks from 0 to n\>
 
 
 
 \<parameter M\>
 
 \<parameter C\>
 
 

 \<x coordanate of base task 0\> \<y coordanate of base task 0\>
 
 \<x coordanate of task 1\> \<y coordanate of task 1\>
 
 ...
 
 \<x coordanate of task n\> \<y coordanate of task n\>


# Results 
 
The results files contain the first frontier of the last generation of each method, i.e. the number of solutions of the first frontier and the value of objetive functions f1 and f2 of every solution. Files can be read as: 
 
 \<number of solutions\>
 
 \<f1 value of solution 1\> \<f2 value of solution 1\>
 
 \<f1 value of solution 2\> \<f2 value of solution 2\>
 
 \<f1 value of solution 3\> \<f2 value of solution 3\>
 
 ...
 



