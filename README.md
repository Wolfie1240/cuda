# Monte Carlo Simulation of Golf Balls

This project simulates golf ball trajectories using a Monte Carlo method on a CUDA-enabled GPU. It computes the probability of a golf ball landing within a target radius using parallel computation.


## Compilation and Execution
Ensure you have CUDA installed and a compatible GPU.  
Compile and execute the program:  
   ```bash
   nvcc -o monte_carlo monte_carlo.cu  
   *OR*  
   nvcc -DNUMTRIALS=262144 -DBLOCKSIZE=128 -o monte_carlo monte_carlo.cu  ~ If you want to control Number of trials and blocksize  
   ./monte_carlo
   ```
  Output:  
           Probability: Percentage of successful trials.  
           Performance: Mega-trials per second.  
  

 

