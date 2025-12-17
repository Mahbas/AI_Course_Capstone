# AI_Course_Capstone

This repository contains my Black-Box Optimisation (BBO) capstone project, completed as part of a multi-stage machine learning programme. The project simulates a real-world optimisation challenge in which the goal is to maximise eight unknown (black-box) functions under strict evaluation constraints.

Each black-box function represents a realistic optimisation scenario where evaluations are expensive and the underlying function is unknown, such as problems encountered in robotics, scientific discovery or system tuning. The functions vary in dimensionality from 2D to 8D, increasing in complexity over the course of the project.

At the start of the capstone, each function is provided with ten initial observations. Across ten sequential rounds, only one new query per function per round is permitted. After each submission, the newly observed outputs are added to the dataset, and the optimisation strategy is revised accordingly. This iterative process mirrors how optimisation is approached in real research and industrial settings, where decisions must be made with limited and gradually expanding information.

Rather than aiming for perfect global optima, the focus of this project is on principled decision-making, exploration–exploitation trade-offs and transparent reasoning. A range of strategies were explored, including exploratory sampling, local exploitation of promising regions and data-driven adaptation as patterns emerged across rounds. Weekly reflections document how insights from previous evaluations informed subsequent decisions.

To support reproducibility and responsible ML practice, this repository includes:

  - A datasheet documenting the query history and function evaluations generated during the project [Datasheet](Datasheet.md)

  - A model card describing the optimisation strategy, assumptions, performance and limitations [Model Card](ModelCard.md)

  - Supporting notebooks and analysis used to guide decision-making across rounds

The project emphasises that in black-box optimisation, success is defined not only by the final numerical outcome, but by the clarity, rigour and adaptability of the optimisation process itself.

Key Tools and Libraries

The following tools and libraries were used throughout the capstone project:

  - Python – core programming language for experimentation and analysis

  - NumPy – numerical computation, random sampling and array operations

  - Pandas – data storage and manipulation of query histories and function evaluations

  - Matplotlib / Seaborn – visualisation of function behaviour, trends and exploration patterns

  - Scikit-learn – surrogate modelling and baseline models where applicable

  - Gaussian Process concepts – used conceptually to guide exploration–exploitation strategies

  - Acquisition functions – Upper Confidence Bound (UCB) and Expected Improvement (EI)

  - Manual feature transformations – e.g. log-scaling for large dynamic ranges

  - Git & GitHub – version control, documentation and reproducibility
