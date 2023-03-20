# STRSP_multi_objetive

This repository contains all instances and results of the tests presented in the subscribed paper "Scheduling technicians and tasks through a multi-objective Biased Random-Key Genetic Algorithm" by th eauthors R. B. Damm,  J. A. R. Merino, A. Chaves and D. P. Ronconi. The repository is stuctured as follows:



Folder "Instancias" contains all the instances used for testing. Each file ".txt" represent an instance and the name of each file is ... . Folder "Resultados" contains te result of each algorithm tested in each subfolder "BRKGA-QL", "NSGA-II" and ^SPEA2". The name of fles si <Arlgorithm>...



# Instances 

The generated instances are based on the reference instances of Solomon (1987) for the vehicle routing problem with time windows. The following parameters were varied: i ) length of tasks’ time windows, ii ) type of geographical distribution, and iii ) number of tasks and technicians as follows. Time windows were classified into three different scenarios, namely, short, long, and random; a short time window [e, ℓ] corresponding to ℓ−e ∈ {1.5h, 2h, . . . , 3.5h}, a long time window corresponding to ℓ − e ∈ {6.5h, 7h, . . . , 9h}, and a random time window corresponding to ℓ − e ∈ \{1.5h, 2h, . . . , 9h\}. Geographical distributions were classified as (R) random uniform distribution, (C) clustered distribution, and (RC) semi-clustered distribution as suggested in Solomon (1987). There were considered eleven combinations of a number of tasks and technicians as depicted in Table 2, totaling 99 = 3 × 3 × 11 instances. The last column of Table 1 will be further described in Section ??. In all cases, parameters were randomly generated with uniform distribution within the following sets: (a) wi ∈ {1, 2, . . . , 10}, i ∈ S; (b) pi ∈ \{30min, 35min, . . . , 120min\}, i ∈ S; (c) ei ∈ \{7h, 8h, . . . , 19h\}, i ∈ S; (d) ℓi ∈ {ei +1.5h, ei +2h, . . . , ei +3.5h}, ℓi ∈ {ei +6.5h, ei +7h, . . . , ei +9h}, or ℓi ∈ {ei + 1.5h, ei + 2h, . . . , ei + 9h} depending on the type of the tasks’ window length, i ∈ S; (e) ak ∈ {7h, 7.5h, . . . , 12h}, k ∈ K; and (f ) for all i ∈ S, sik = 1 for k ∈ Ki and sik = 0 for k ∈ K \ Ki, where |Ki| is a random number in {1, . . . , m} (with discrete uniform distribution) and Ki ⊆ K is a random subset. For the generation of the tasks’ locations, see Solomon (1987). Taillard’s random number generator and seeds were used to generate discrete random numbers with uniform distribution (see Taillard (1993)). The other parameters associated with the technicians were defined as follows. The end of the daily work was set as bk = ak + 9h, lunch break has a duration of 1 hour, i.e. pn+k = 1h, with a time window given by [en+k, ℓn+k] = [ak + 3h, bk − 3h] for all k ∈ K.

Each instance file is structured as:
 
 \<number of task\> 
 
 \<number of technician\>


...





