# ECON408: Computational Methods in Macroeconomics

- **(3 credits course)** Computational tools used in macroeconomics and financial economics including applications to unemployment, inequality, asset pricing, and economic growth
- **Instructor:** jesse.perla@ubc.ca
- **Prerequisites:** One of ECON 301, ECON 304, ECON 308 and one of ECON 323, CPSC 103, CPSC 110, MATH 210, COMM 337 and one of MATH 221, MATH 223.
- **Textbook:** Posted lecture notes based on the  Online, open-source textbook [Quantitative Economics with Julia](https://julia.quantecon.org/) by Jesse Perla, Thomas J. Sargent and John Stachurski 
  - In cases where material in those lectures is too advanced, we will choose a subset and adapt lecture materials to be appropriate for the level
  - The textbook includes both theory and code, and a set of [Jupyter notebooks](https://github.com/QuantEcon/lecture-julia.notebooks).
- **TA and Office Hours:** Posted on Canvas

## Course Overview

This is a course in computational tools used in macroeconomics.  You are expected to have some proficiency in Matlab, Python, Julia, and similar languages as fulfilled in the prerequisites (i.e., ECON 323, CPSC 103, CPSC 110, MATH 210, COMM 337).  Even intermediate knowledge of R is typically not sufficient.

Models in macroeconomics and financial economics are constructed from a core set of tools which model each agents' decisions while maintaining an internal consistency between the decisions of complicated distributions of other agents in an economy.

Some of the common features of models in macroeconomics and financial economics include:

1. __dynamic and forward looking decisions__: If I consume less today, I can save more for tomorrow;
2. __randomness and uncertainty about the future__: If reject a job offer, I am not sure when the next offer will occur;
3. __prices and resources reflecting the collective decisions of other agents__: The wage I am offered depends on the number of similar workers I am competing with, the intensity which the unemployed search for jobs, and the demand for my skills from firms;
4. __social learning from other agents' with information aggregated through prices__: If many others consider a particular equity or bond asset a good buy, then I can infer this by the price of the asset itself; and
5. __distributions and heterogeneity in the economy influencing decisions and prices__: If the distribution of income is askew and there are many poor agents living hand-to-mouth, government policy such as sending out stimulus cheques has a different effect on inflation and consumer welfare than if every person had similar incomes.

The interaction between these makes it difficult to do counter-factual experiments with "partial-equilibrium" in macroeconomics---i.e., changing one price or element of the model in isolation---because of the interconnection of decisions, prices, and distributions.   However, by writing formal models in mathematics, we can conduct policy experiments and interpret data while still ensuring all of these conditions for self-consistency.  Using precise mathematical language will (1) uncover unanticipated consequences implicit in your assumptions; (2) keep everyone honest; (3) provide a framework to investigate changes in assumptions; and (4) allow disciplined nesting of models to add enough "reality" for quantitative analysis.

The downside is that while this set of mathematical tools provides a rich set of economic theories that can be explored and tested against the data, the inherent difficulty of dynamic models means that we may usually need to solve them approximately and on a computer.

This course is designed to jointly explore these sorts of theoretical models in conjunction with the computational tools to solve and simulate them.  We will learn using the Julia programming language—--a modern language for scientific and technical computing. If you have an existing background in Python or Matlab from other courses you will find that Julia compliments those skills.

### Learning Outcomes

By the end of the course, you will be able to

1. program using tools from linear algebra, probability, and optimization
2. simulate and analyze stochastic processes for the purpose of understanding the evolution of the wealth distribution
3. describe economic dynamics as a linear state space model and solve them numerically
4. implement and analyze Markov chains, and apply them to models of unemployment and asset pricing
5. investigate the role of general equilibrium and prices in aggregating information and reflecting the real economy
6. define economic problems recursively, such labor market search and consumption savings models, and solve them numerically
7. define and implement dynamic models of growth

## Assignments and Assessment

The only way to learn how to apply programming to economic problems is practice. To aid this, a significant portion of the assessment will be in the form of problem sets.

The weighting in the grade is:

- 6-8 problem sets: 20% (total)
- Midterm exam: 30%
- Final exam: 50%

Both the midterm and final examinations will be done in a computer lab or on your own computer in class and contain a mixture of theory and computational questions.

The problem sets will start off short and easy to help those with less programming experience, and then build in complexity.  This is a macroeconomics class, not a programming class, so you should not be worried about the quantity of code required.

**Missed Exam Policy:** You are responsible for ensuring that you take these exams as scheduled; no make-up exams will be given.
- Missing a midterm for **ANY** acceptable reason will result in its weight being automatically transferred to the final exam.
- The final exam date will be announced by Student Services about half-way through the term.
- There is no make-up final. Travel plans and/or cheap tickets are not a reason to miss the final. If you have a medical or other compelling reason why you cannot take the final exam at its scheduled time you must follow the formal process and get an Academic Concession from your Faculty Advising Office (see below)


### Computational Infrastructure and Programming Language

While you will have experience with another programming language such as Python or Matlab from your prerequisites, this course will be taught using [Julia](https://julialang.org/).  Beyond being an excellent language for technical computing and popular among macroeconomists and researchers in finance, Julia provides a new set of programming principles that will broaden the your knowledge of computing.  This will help you by both providing a better differentiated resume, broader skills, and more opportunities to work as a research assistant for researchers requiring significant computational expertise.

You can install Julia on your laptop by following [these instructions](https://julia.quantecon.org/getting_started_julia/getting_started.html).  While one can use Julia entirely from just Jupyter notebook, we will also introduce basic [GitHub](https://github.com/) and [VS Code](https://code.visualstudio.com/) usage as well to help broaden your exposure to computational tools.

## Course Outline

We will cover the following topics, with the later topics only if time-permits.

### Basic Programming Review

   - Topics include: [Getting Started](https://julia.quantecon.org/getting_started_julia/getting_started.html) and [Julia Essentials](https://julia.quantecon.org/getting_started_julia/julia_essentials.html)
   - At the end of the section you will have reviewed the basic setup of the Julia programming language and can comfortably accomplish simple tasks as they would in to Python or Matlab.

### Linear algebra and basic scientific computing

   - Topics include [Arrays and Related Types](https://julia.quantecon.org/getting_started_julia/fundamental_types.html) and related topics in implementing [Linear Algebra](https://julia.quantecon.org/tools_and_techniques/linear_algebra.html).  In addition, you will review [Optimizers and Solvers](https://julia.quantecon.org/more_julia/optimization_solver_packages.html).
   - Interested students can review bonus material in [Generic Programming](https://julia.quantecon.org/getting_started_julia/introduction_to_types.html) but it wouldn't be required or tested.
   - At the end of the section you will feel comfortable working with matrices, vectors, and arrays; solving linear systems and calculating eigenvalues; optimizing unconstrained and constrained functions; and solving systems of equations.

### Geometric Series and Discrete Time Dynamics

  - Topics include [Geometric Series](https://julia.quantecon.org/tools_and_techniques/geom_series.html) and [Dynamics in One Dimension](https://julia.quantecon.org/introduction_dynamics/scalar_dynam.html)
  - At the end of the section you will understand how to calculate present discounted values, work with Keynesian money-multipliers, and fixed points of dynamic Models.

### Stochastic Processes and Dynamics of Wealth and Distributions

  - Topics include [AR1 Processes](https://julia.quantecon.org/introduction_dynamics/ar1_processes.html) and [Wealth Distribution Dynamics](https://julia.quantecon.org/introduction_dynamics/wealth_dynamics.html)
  - At the end of the section you will better ergodic distributions, measures of inequality, and how to simulate the dynamics of the wealth distribution.

### Linear State Space Models

  - Topics include [Linear State Space Models](https://julia.quantecon.org/introduction_dynamics/linear_models.html)
  - At the end of this week you will understand how to describe processes such as asset pricing and consumption smoothing as linear-state space models, simulate them, and calculate present-discounted values using those stochastic processes.

### Permanent Income Model

  - Topics include [The Permanent Income Model](https://julia.quantecon.org/dynamic_programming/perm_income.html)
  - At the end of the section you will understand how to implement the classic consumption-savings model with linear-quadratic preferences in the LSS framework of the previous lecture, and to simulate permanent and transitory shocks to income.

### Markov Chains

  - Topics include [Finite Markov Chains](https://julia.quantecon.org/introduction_dynamics/finite_markov.html)
  - At the end of the section you will understand how to describe discrete-state stochastic processes as Markov chains and simulate models of unemployment for a worker.

### Models of Unemployment

  - Topics include the [Lake Model of Employment and Unemployment](https://julia.quantecon.org/multi_agent_models/lake_model.html)
  - At the end of the section you will build on the previous tools of Markov chains to look at a aggregated models of employment and unemployment in the economy.

### Rational Expectations and Firm Equilibria

  - Topics include [Rational Expectations Equilibrium](https://julia.quantecon.org/multi_agent_models/rational_expectations.html)
  - At the end of the section you will understand the core "big K, little k" insight for implementing rational expectations equilibria and apply it to models of firm dynamics.

### Asset Pricing

  - Topics include [Asset Pricing with Finite State Models](https://julia.quantecon.org/multi_agent_models/markov_asset.html)
  - At the end of the section you will understand pricing assets with payouts following a Markov-chain as derived in the previous lectures.

### Lucas Trees

  - Topics include [Asset Pricing with Finite State Models](https://julia.quantecon.org/multi_agent_models/markov_asset.html) and some of [The Lucas Asset Pricing Model](https://julia.quantecon.org/multi_agent_models/lucas_model.html)
  - At the end of the section you will understand how to price assets with continuous rather than discrete payoffs.

### Recursive Equilibria and the McCall Search Model

  - Topics include [The McCall Search Model](https://julia.quantecon.org/dynamic_programming/mccall_model.html)
  - At the end of the section you will be able to define and solve basic models of labor market search.

<!--### Cake Eating Problem (LO6)

  - Topics include [Optimal Savings](https://python.quantecon.org/cake_eating_problem.html) and [Numerical Methods for Solving the Cake Eating Problem](https://python.quantecon.org/cake_eating_numerical.html)
  - At the end of the section you will be able to implement simple value-function iteration to solve a dynamic programming problem with a continuous set of decisions.
### Cass Koopmans/Neoclassical Growth

  - Topics include [Cass Koopmans Planning Problem](https://julia.quantecon.org/multi_agent_models/cass_koopmans_1.html)
  - At the end of the section you will be able to solve for the transition dynamics of the planning problem for the Cass Koopmans/neoclassical growth model.
  

### Optimal Growth Model (LO7)

  - Topics include [Stochastic Optimal Growth Model](https://julia.quantecon.org/dynamic_programming/optgrowth.html)
  - At the end of the section you will be able to solve growth models with a single type of good and stochastic productivity.
  - **Problem Set 6 Due** - solving stochastic dynamic programming and simulating  transition dynamics of growth models.
--> 


## General Policies

### Policy for Academic Concessions:
Sometimes, things happen during the course of a semester that can affect your ability to succeed.  There are three main categories:
- Medical – i.e. you got sick and missed class or a chronic illness got worse
- Compassionate – i.e. a friend or close relative had something bad happen to them, or something bad happened to you.
- Conflicting Responsibilities – i.e. something happened in your personal life which is affecting your ability to do the work, like childcare falling through
You can read more about specific examples and the whole policy at:
http://www.calendar.ubc.ca/vancouver/index.cfm?tree=3,48,0,0

In all of these cases, UBC’s policy is to allow you to request an academic concession.  Our policy is that all requests for academic concession on exams should be handled through your faculty Advising office (unless your office advises otherwise).  This is so that we can centrally track requests for concession and ensure they are fairly administered; it also helps protect your privacy.  You can find the procedure here, for Arts:

https://students.arts.ubc.ca/advising/academic-performance/help-academic-concession/

If you need a concession, you should immediately speak to Advising, who will follow-up with the instructor to handle the academic side of things.  In-term concessions, which handle things like missed assignments or deadlines, are handled usually by extending the deadline or adjusting the final grading of the course (e.g. omitting an assessment).  Alternative forms of assessment may also be used if suitable and recommended by Advising.
•	Concessions need to be made in a timely fashion, which I will define as “within 2 weeks of the missed assessment” unless this is not reasonable.
You are also welcome to speak to the instructor regarding your issue; I’m here to support you and help you get through things and be successful.  If you’re not sure if it’s something you should/could get a concession for, I can also give you a quick sense of what Advising will likely suggest if you’re unable to make an appointment immediately. 


### Student Success:

UBC provides resources to support student learning and to maintain healthy lifestyles but recognizes that sometimes crises arise and so there are additional resources to access including those for survivors of sexual violence. UBC values respect for the person and ideas of all members of the academic community. Harassment and discrimination are not tolerated nor is suppression of academic freedom. UBC provides appropriate accommodation for students with disabilities and for religious, spiritual and cultural observances. UBC values academic honesty and students are expected to acknowledge the ideas generated by others and to uphold the highest academic standards in all of their actions. Details of the policies and how to access support are available here: https://senate.ubc.ca/policies-resources-support-student-success/.

### Policy on sharing course materials:

All the materials provided to you as part of this course are protected by copyright. All assignment instructions, quiz questions and answers, discussion questions, announcements, lecture slides, audio/video recordings, Canvas modules, and any other materials provided to you by your instructor or in the textbook are for use only by students enrolled in this course this term. Sharing any of these materials beyond this course, including by posting on file-sharing websites (e.g., CourseHero, Google Docs) is a violation of copyright law and an academic offence. Copying and pasting sentences from the lecture notes or the textbook (e.g., definitions) into for-profit software (e.g., Quizlet) is likewise a violation of copyright law, and an academic offence. Violations of this policy will be treated according to the provisos of the Code of Student Conduct. For further information about copyright law, please refer to (https://copyright.ubc.ca/students/).

### Policy on Academic Honesty:

It is the policy of the Vancouver School of Economics to report all violations of UBC’s standards for academic integrity to the office of the Dean of Arts. All violations of academic integrity standards will result in a grade of zero on the relevant assessment (exam, paper, assignment etc.).  Students who do not have a previous offence may have the option to enter into a diversionary process with the Dean of Arts to resolve their misconduct (https://academicintegrity.ubc.ca/diversionary-process/). Any student who has a previous academic offence will be referred to the President’s Advisory Committee on Student Discipline (PACSD) (https://universitycounsel.ubc.ca/homepage/guides-and-resources/discipline/). PACSD may impose additional penalties including: a transcript notation indicating that the student has committed an academic offence, zero in the course, and/or suspension or expulsion from the University. You are personally responsible for understanding and following the UBC’s policies for academic integrity: https://vancouver.calendar.ubc.ca/campus-wide-policies-and-regulations/academic-honesty-and-standards. A Canvas module has been made available you for this purpose titled “Avoiding Academic Misconduct”. It is your responsibility to read the materials in that module before submitting any work in this course. Speak to your instructor if you have any questions regarding the standard for academic integrity at UBC and/or the VSE polices on academic misconduct.

### Policy on Academic Concessions:

There are only three acceptable grounds for academic concessions at UBC: unexpected changes in personal responsibilities that create a schedule conflict; medical circumstances; and compassionate grounds when the student experiences a traumatic event, sexual assault, or death in the family or of a close friend. Academic concessions for graded work and exams are granted for work that will be missed due to unexpected situations or circumstances. Situations that are expected (such as time constraints due to workload in other courses) or are predictable (such as being scheduled for paid work) are not grounds for academic concession.

Requests for academic concessions should be made before the due date for that graded work and/or the writing of the exam. UBC policy does not allow for concessions to students who have missed work because they have registered for a course after the due date for that work. You can read more about the rules for academic concessions here: https://students.ubc.ca/enrolment/academic-learning-resources/academic-concessions. Students in the Faculty of Arts who require a concession can apply for concessions using this form here: https://students.air.arts.ubc.ca/academic-concession-form/. Students in other Faculties should consult their faculty website on academic concessions. Please note that the role of the faculty advising office is to review the evidence and to either support or not support concession requests. The final decision to grant the request always rests with your instructor.

### Policy on the Use of AI Learning Tools:

The specific rules for the use of AI tools are at the discretion of the course instructor. Those rules might change over the course of the term as new technologies become available. Changes to those rules might change the content of assessments and the way that your work is evaluated. If no written instructions on the use of AI tools have been provided by the instructor, the use of all AI tools is strictly prohibited in the course. Where the written instructions permit the use of AI tools, that usage must be documented and attributed within your assessment(s). Students are responsible for all factual inaccuracies that are created by the use of AI tools. Please speak to your instructor if you have further questions about the ways in which AI technology use is permitted in this course.

### VSE Policy Prohibiting the Hiring of Tutors: 

The Vancouver School of Economics expressly prohibits any student from hiring a tutor and/or editor to assist with any portion of written work or academic research. If at any point you feel in need of additional writing support, please speak with your instructor and/or arrange for a writing consultation with UBC’s Centre for Writing and Scholarly Communication (https://writing.library.ubc.ca/). Additionally, you have access to research support through the UBC Library:  https://guides.library.ubc.ca/econ and https://guides.library.ubc.ca/econ490.

Any student who hires a tutor and/or editor to assist with any portion of written work or academic research will be given a zero on that component of the course and will be reported to the Dean’s office for academic misconduct (please see Policy on Academic Honesty).
