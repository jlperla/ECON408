# ECON408: Computational Methods in Macroeconomics, Winter 2024
Open as website [here](https://jlperla.github.io/ECON408/)

It is strongly suggested to get GitHub's [student developer pack](https://education.github.com/pack) which gives you lots of free stuff (and even access to the AI [GitHub Copilot](https://docs.github.com/en/copilot/quickstart) ). Optionally, select `Watch` at the top of this repository to be alerted to all file changes

## Syllabus
See [here](syllabus.md) for more details, a course outline, and grading information.

## Problem Sets and Exams

1. **Due Midnight PST on January 17th** - [Problem Set 0](/problem_sets/problem_set_0.ipynb)
   - This is a pass/fail problem set (i.e., hand it in you pass!) just to ensure you have setup your computer properly 
2. **Due Midnight PST on January 30th** - [Problem Set 1](/problem_sets/problem_set_1.ipynb)
3. **Due Midnight PST on February 6th** - [Problem Set 2](/problem_sets/problem_set_2.ipynb)
4. **Due Midnight PST on February 13th** - [Problem Set 3](/problem_sets/problem_set_3.ipynb)
5. **Due Midnight PST on TBD** -  Problem Set 4 <!-- [Problem Set 4](/problem_sets/problem_set_4.ipynb) -->
6. **Review February 26th** - Midterm Practice Problems  <!--[Midterm Practice Problems](/problem_sets/midterm_practice_problems.ipynb) -->
7. **February 28th** - MIDTERM EXAM IN CLASS
8. **Due Midnight PST on TBD** -  Problem Set 4 <!-- [Problem Set 4](/problem_sets/problem_set_4.ipynb) -->
9. **Due Midnight PST on TBD** -  Problem Set 5 <!-- [Problem Set 5](/problem_sets/problem_set_5.ipynb) -->
10.  **Due Midnight PST on TBD** -  Problem Set 6 <!-- [Problem Set 6](/problem_sets/problem_set_6.ipynb) -->
11. **Reviewing TBD** - Final Practice Problems <!-- [Final Practice Problems](/problem_sets/final_practice_problems.ipynb) -->

All problem set solutions should be submitted on Canvas directly as a `.ipynb` file with instructions embedded.


## Lectures
See [here](https://jlperla.github.io/ECON408/index.html) for links to all materials.

1. **January 8th** - Introduction, course overview, VSCode Intro to Julia
   - **Lecture Notes**: [Course Overview and Computational Environment](https://jlperla.github.io/ECON408/lectures/intro.html)
   - **References**:
     -  [Julia Overview](https://julia.quantecon.org/getting_started_julia/getting_started.html)
     -  First sections of [Julia by Example](https://julia.quantecon.org/getting_started_julia/julia_by_example.html)
     -  [Essentials](https://julia.quantecon.org/julia_essentials.html)
     -  [Fundamental Types](https://julia.quantecon.org/getting_started_julia/fundamental_types.html)
2. **January 10th** - Introduction to Fixed Points and Geometric Series and start of Asset Pricing applications
   - **Lecture Notes**: [Geometric Series, Fixed Points, and Asset Pricing](https://jlperla.github.io/ECON408/lectures/geometric_series_fixed_points.html)
   - **References**:
     -  Later sections of [Julia by Example](https://julia.quantecon.org/getting_started_julia/julia_by_example.html)
     -  [Geometric Series for Elementary Economics](https://julia.quantecon.org/tools_and_techniques/geom_series.html)     
3. **January 15th** - Continue on applications of Fixed Points and Geometric Series
   - **Lecture Notes**: [Geometric Series, Fixed Points, and Asset Pricing](https://jlperla.github.io/ECON408/lectures/geometric_series_fixed_points.html)
   - **References**:
     -  Later sections of [Julia by Example](https://julia.quantecon.org/getting_started_julia/julia_by_example.html)
     -  [Geometric Series for Elementary Economics](https://julia.quantecon.org/tools_and_techniques/geom_series.html)
4. **January 17th** - Start Dynamics and Introduction to Growth Models
   - **Lecture Notes**: [Deterministic Dynamics and Introduction to Growth Models](https://jlperla.github.io/ECON408/lectures/deterministic_dynamics.html) and contraction mappings in [Geometric Series, Fixed Points, and Asset Pricing](https://jlperla.github.io/ECON408/lectures/geometric_series_fixed_points.html)
   - **References**:
     -  [Dynamics in One Dimension](https://julia.quantecon.org/introduction_dynamics/scalar_dynam.html)
5. **January 22nd** - Solow Model and Stability
   - **Lecture Notes**: [Deterministic Dynamics and Introduction to Growth Models](https://jlperla.github.io/ECON408/lectures/deterministic_dynamics.html)
   - **References**:
     -  [Dynamics in One Dimension](https://julia.quantecon.org/introduction_dynamics/scalar_dynam.html)
6. **January 24th** - Finish Malthusian Model and start AR(1) and Stochastic Dynamics
   - **Lecture Notes**:  [Deterministic Dynamics and Introduction to Growth Models](https://jlperla.github.io/ECON408/lectures/deterministic_dynamics.html) and  [Stochastic Dynamics, AR(1) Processes, and Ergodicity](https://jlperla.github.io/ECON408/lectures/stochastic_dynamics.html)
   - **References**:
     - [AR1 Processes](https://julia.quantecon.org/introduction_dynamics/ar1_processes.html)
     - [LLN and CLT](https://julia.quantecon.org/tools_and_techniques/lln_clt.html)
     - [Continuous State Markov Chains](https://julia.quantecon.org/tools_and_techniques/stationary_densities.html)
7. **January 29th** - Stochastic Dynamics, AR(1), ARMA, and Ergodicity
   - **Lecture Notes**:  [Stochastic Dynamics, AR(1) Processes, and Ergodicity](https://jlperla.github.io/ECON408/lectures/stochastic_dynamics.html)
   - **References**:
     - [AR1 Processes](https://julia.quantecon.org/introduction_dynamics/ar1_processes.html)
     - [LLN and CLT](https://julia.quantecon.org/tools_and_techniques/lln_clt.html)
     - [Continuous State Markov Chains](https://julia.quantecon.org/tools_and_techniques/stationary_densities.html)
8. **January 31st** - Finish Nonlinear Stochastic Dynamics and Start Wealth Inequality
   - **Lecture Notes**:  [Stochastic Dynamics, AR(1) Processes, and Ergodicity](https://jlperla.github.io/ECON408/lectures/stochastic_dynamics.html) and  [Wealth Distribution, Firm Dynamics, and Inequality](https://jlperla.github.io/ECON408/lectures/wealth_distribution_firm_dynamics.html)
   - **References**:
     -  [Wealth Distribution Dynamics](https://julia.quantecon.org/introduction_dynamics/wealth_dynamics.html)
9. **February 5th** - Firm Dynamics, Lorenz Curves and Power Laws
   - **Lecture Notes**:  [Wealth Distribution, Firm Dynamics, and Inequality](https://jlperla.github.io/ECON408/lectures/wealth_distribution_firm_dynamics.html)
   - **References**:
     -  [Wealth Distribution Dynamics](https://julia.quantecon.org/introduction_dynamics/wealth_dynamics.html)
10. **February 7th** - Review of PS1 and PS2 in class
11. **February 12th** - Finish Wealth Distribution, Firm Dynamics, and Inequality and start Linear State Space Models
    - **Lecture Notes**:  [Wealth Distribution, Firm Dynamics, and Inequality](https://jlperla.github.io/ECON408/lectures/wealth_distribution_firm_dynamics.html) and [Linear State Space Models, Asset Pricing, and the Kalman Filter](https://jlperla.github.io/ECON408/lectures/linear_state_space_models.html)
    - **References**:
      - [Wealth Distribution Dynamics](https://julia.quantecon.org/introduction_dynamics/wealth_dynamics.html)
      - [Linear State Space Models](https://julia.quantecon.org/introduction_dynamics/linear_models.html#the-linear-state-space-model)
12. **February 14th** - Linear State Space Models, Asset Pricing, and the Kalman Filter
    - **Lecture Notes**: [Linear State Space Models, Asset Pricing, and the Kalman Filter](https://jlperla.github.io/ECON408/lectures/linear_state_space_models.html)
    - **References**:
      - [Linear State Space Models](https://julia.quantecon.org/introduction_dynamics/linear_models.html#the-linear-state-space-model)
      - [A First Look at the Kalman Filter](https://julia.quantecon.org/introduction_dynamics/kalman.html)
13. **February 19th** - SPRING BREAK
14. **February 21st** - SPRING BREAK
15. **February 26th** - Midterm Review
16. **February 28th** - Midterm
17. **March 4th** - 
18. **March 6th** - 
19. **March 11th** - 
20. **March 13th** - 
21. **March 18th** - 
22. **March 20th** - 
23. **March 25th** - 
24. **March 27th** - 
25. **April 1st** - STATUTORY HOLIDAY
26. **April 3rd** - 
27. **April 8th** - 
28. **April 10th** - 


## Software and Programming Environment
For the computational environment, it is strongly suggested to install [VS Code](https://code.visualstudio.com/) as well as Jupyter.  Familiarity with those tools will make it easier for future work in industry or as research assistants.  See [here](https://julia.quantecon.org/getting_started_julia/getting_started.html) to setup your environment.

While we will be using a computer for simulations and numerical solutions to our models, this is an economics course.  If you have the prerequisites, then **do not be scared off by the programming requirements!**  Relative to many classes, the coding will be kept simple.  The hard part will be the economic and finance theory.