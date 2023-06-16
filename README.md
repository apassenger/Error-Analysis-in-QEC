# Error-Analysis-in-QEC
From experiemntal data to error p

It is commonly believed in the community that single- and two-qubit fidelities are the correct metrics to quantify how good quantum gates are. While this argument has some validity, gate fidelity alone may not accurately reflect whether a gate is truly perfect or if unitary errors are present. Moreover, there is a common misunderstanding regarding gate fidelities. For example, if we say that our gate has a 99% fidelity, it is often thought that the error in the system is equal to the infidelity (in this case, 1-99=0.01). However, this is incorrect. The amount of error in the system depends on the type of error present in the lab, and our error rate is always higher than our infidelity. The objection is, then, often raised, 'But they are close enough.' However, this statement is not accurate. It is unclear what is being compared and what the benchmark is for determining what is 'close enough'.
Although one- and two-qubit fidelities may be seems close enough when we compared the error rate of the one and single qubit gate and infidelity of one and two qubit gates, they do not provide sufficient information about the total error rate of parity check circuits used in quantum error correction. This requires a more complex process than simply adding or multiplying infidelities or error rates. Our paper (link) explains this process in detail.

We have created a code repository where we share software that takes experimental process matrices and performs the following:

        Step 1: Calculates the real error rates for each individual quantum gate
   
        Step 2: Calculates the perfection rate and the total error rate for the oarity check circuit according to the formula (S.26) in the paper,
        using the error rates from step 1. This part is explained in very detail in the paper.

We demonstrate numerically that relying solely on single- and two-qubit fidelities is not sufficient for having self-confidence in fault-tolerant quantum computing. To use this code for your system, you will need to provide your own experimental and ideal process matrices. Please feel free to contact us with any further questions, and if you use the code, please cite our paper and software.
For software:

Üstün, G., Morello, A., & Devitt, S. (2023). Error Analysis in the context of Quantum Error Correction (Version 1.0.0) [Computer software]. https://github.com/apassenger/Error-Analysis-in-QEC

or

@software{Ustun_Error_Analysis_in_2023,
author = {Üstün, Gözde and Morello, Andrea and Devitt, Simon},
month = apr,
title = {{Error Analysis in the context of Quantum Error Correction}},
url = {https://github.com/apassenger/Error-Analysis-in-QEC},
version = {1.0.0},
year = {2023}
}


For paper: https://arxiv.org/abs/2306.08849

This project shows how to find the real error rate for individual gates from experiemental data. 

Then, the perfection rate for the XX parity check circuit is computed. 
