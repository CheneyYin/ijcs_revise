#### 1. Writing mistakes

1. At section 1(***Introduction***), 

   - The "==*becomesan*==" should be revised to "**becomes an**" one the 1st paragraph. 
   - The "==*areseveral*==" should be revised to "**are several**" in the 2nd paragraph.
2. At section 2(***Literature Survey***), 

   - The "==*worksrelated*== should be revised to "**works related**" in the 1st sentence.
3. At section 3.1(***System model***), 

   - The "==Allocationof==" should be revised to "**Allocation of**" in the 3rd sentence.
   - The "==consumein==" should be revised to "**consume in**", 
   - The "==computingPhysical==" should be revised to "**computing Physical**" in the 5th sentence.
   - The "==wholeallocated==" should be revised to "**whole allocated**" in the description of ***Request/task Queue***.
   - The "==Afterthat==" should be revised to "**After that**" in the description of  ***Cloud Service Providers***.
   - There are some typography problems in the description of ***Physical Machine Manager (PMM)***.
   - The "==TargetVMwith==" should be revised to "**Target VM with**" in then description of ***Virtual Machine Manager (VMM)***.
4. At section 3.2(***Migration process of virtual machine***), 

   - The "==Machineswith==" should be revised to "**Machines with**".
   - The "==decreasethe==" should be revised to "**decrease the**".
   - The "==consumein==" should be revised to "**consume in**".
   - The "==theNPHard==" should be revised to "**the NP Hard**".
   - The "==machinewhich==" should be revised to "**machine which**".
   - The "==storae==" should be revised to "**storage **".
5. At section 3.2.1(***Generalized Backtracking Regularized Adaptive Matching Pursuit Algorithm (GBRAMP) for VM migration***),
   - The "==GBRAMPis==" should be revised to "**GBRAMP is**".
6. At section 3.3(***Virtual machine placement***),
   - The "==*$id$ is represented as then busy state of PM*==" should be revised to "**$id$ is represented as then idle state of PM**".
   - The "==fewoptimization==" should be revised to "**few optimization**".
7. At section 4(***Result and Discussion***),
   - The "==likeSCA-ALO-VMA-CC==" should be revised to "**like SCA-ALO-VMA-CC**".

#### 2. Literature citation

1. At section 3(***Proposed Methodology***), the first sentence cites the literature 28 & 29, but the references of these literatures are the same one.
2. At section 3.2.1(***Generalized Backtracking Regularized Adaptive Matching Pursuit Algorithm (GBRAMP) for VM migration***), 

   - What is the *Generalized Backtracking Regularized Adaptive Matching Pursuit Algorithm*? You should introduce more details and provide some key citations of it. 
3. At section 3.3.1(***Adaptive β-Hill Climbing Algorithm for optimizing parameters of VM placement***),
   - What is the *Adaptive β-Hill Climbing Algorithm*? Please add some key citations of it.

#### 3. Equation

1. In equation (1), $PW_{Min}$ may be equivalent to $P_{id}$. Because $UT \in [0,1]$, $UT\% \in [0\%, 1\%]$ . Equation (1) should be revised to 
   $$
   PW^{C\_S}_i = [(PW_{Max} - P_{id})] \times UT^{CPU}_{i} + P_{id}
   $$

2. In equation (2), what does the $PM^f_j$ mean? It may be revised to $PM^f_i$.

3. In the description of equation (1) and (2), you set $n$ represent the number of VMs and $m$ represent the number of PMs. But it conflicts with equation (2). In equation (2), $\sum^m_j VM^f_j \times x_{ji}$ maybe revised to $\sum^n_j VM^f_j \times x_{ji}$.  Equation (3) also has a similar problem.

4. What does the $x_{ji}$ mean in equation (2)? Are $x_{ji}$ and $\beta_{ji}$ the same concept?

5. What does the $d$  mean in equation (3)?

6. In the description of equation (4), what does the $VM^{PE}_j$  mean? Dose it mean ***processing elements requested through the $VM_j$***? If true, your description is out of order.

7. In equation (11), $Threshold = \beta + (1 - \beta)$, so $Threshold = 1$?

8. In equation (12), what does the $b_{PM}$ mean?

9. Are equation (14) and equation (1) the same concept?

10. In equation (15) and (17), what does the $y_{PM}$ mean?

11. In equation (16) and (17), whate does the $+\in$ mean?

12. In equation (17), why use bandwidth to evaluate resource consumption instead of using **storage**? ***The bandwidth resource never mention in the previous content***.

13. In equation (26), the $\beta$ as one symbol has appeared many times. Please use different symbols to represent different concepts.

14. In equation (29-32), what does the $k^{'}$ mean?



#### 4. Experiment

1. The **latency** should be as one important metric to evaluate algorithms performance. The meta-heuristics are generally higher time complexity. The latency metric can evaluate production availability.
2. Did the experiment use workloads collected in a real cluster environment? If not, please provide details of the workload.
3. Please provide specifications of Virtual Machines and Physical Machines.
4. The following classic algorithms should be compared,
   - MM, MBFD presented in (***Beloglazov A, Abawajy J, Buyya R. Energy-aware resource allocation heuristics for efficient management of data centers for cloud computing[J]. Future generation computer systems, 2012, 28(5): 755-768.***)
5. According to experiment result, ***GBRAMPA-AβHCA-VMA-CC*** method is better than compared algorithms.  How are these performance advantages achieved? What design of ***GBRAMPA-AβHCA-VMA-CCA*** enables it to achieve such performance? The results of the experiment can only be used to verify that your design works. Please provide more analysis to prove that your design works.



#### 5. Summary

1. This manuscript has many writing mistakes. 
2. Regarding the system model design, the mathematical abstract modeling is not rigorous. There are many formula symbols with ambiguous explanations. Even some of the equations were wrong. Some symbols are conflicting.
3. This manuscript does not provide a formal description of the algorithm.
4. The use of **meta-heuristic algorithms** to solve virtual machine migration and allocation problems is uninspiring, and **enough research has been done on this topic**.
5. The related work part cannot fully introduce the current research status and future trends of virtual machine resource management.
6. This manuscript does not provide detailed experimental setup.
7. This manuscript does not provide a novel research perspective of virtual machines manage.
