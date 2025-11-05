# Calculus x Physics Learning Module Design
This Repository contains prototype design of online learning modules at the intersection of University level Calculus and Physics.

## Structure of Online Learning Modules
* This repository contains one prototype learning unit with 3 Calculus focused learning modules and 2 Physics focused learning modules. Each module contains both instructional materials and an expandable isomorphic problem bank with 10+ problems, both created with the assistance of generative AI.
    * Calculus focused modules:
        * Topic: Derivative as the limit of differences
        * Each problem in isomorphic problem bank builds a math model for a physically feasible situation.
        * Instead of always using y=f(x), math expression used in each problem is context appropriate.
    * Physics focused modules:
        * Topic: Velocity and Acceleration in 1D
        * Involve more sophisticated calculus than most existing Physics I textbook
        * Connects naturally from math modules
* The formative isomorphic problem banks and the instructional content are both generated with the assistance of Generative AI (ChatGPT).
## File Structure.
* Each module is contained in its own folder and contain one sub-folder and four files
    * **A markdown** file (for example: instruction.md), containing the AI generated markdown for the instructional text and image.
    * **An instruction.pdf** file, which is the pdf preview of the instructional content.
    * **A .yml yaml** file. Contains the complete formative problem bank, and the generation prompts.
    * **A problembank.pdf** file which provides a preview of some of the problems in the problem bank. =
    * **A Figures** folder, containing the AI generated images used in the instruction.
## Yaml storage format:
* Each problem bank file contains GenAI prompts for future expansion or replication.
* This yaml format is based largely on https://ybe.readthedocs.io/en/latest/

## Acknowledgement
The contents of this repository was created by Dr. Zhongzhou Chen with the generous support of the Gates Foundation.
