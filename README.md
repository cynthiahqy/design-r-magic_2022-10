# Design R Magic

<!-- badges: start -->

<!-- badges: end -->

This repository contains my quarto slides and discussion notes from my talk about Designing R Packages at the Monash EBS Data Science Research Software Study Group on Oct 4, 2022.

Discussion Notes:

-   Is the dependency you want to use likely to be maintained? -- who is author, how popular is the package?
-   Be careful with `{usethis}` since it hides what's happening underneath and can make it debugging difficult. Maybe consider learning how to do things the hard way and then using the convenient wrappers offered by `{usethis}`
-   Experimenting with different use cases will help refine your idea of what your package should offer, and how it should offer that functionality.
-   Completely redesigning functions and features is normal! Sometimes it will turn out that code which uses your package is UGLY. 
-   When planning and/or redesigning functions, try writing out what you want user code to look like -- e.g. how functions should pipe together etc.
-   Ideas for organising scripts and artefacts from initial prototyping stage:
    -   use vignettes as scratch pads
    -   maintain two packages -- one for "finalised"" functions and another one for experimentation or project specific workflows
    -   use separate git branches (but also remember no one is judging the stray scraps of code on your github)
    -   create a concept glossary to define the abstractions your package offers, and to track the different names you've considered using to refer to new concepts (e.g. for a function that does something to some input data, you might have used a variety of argument names in your code like: "origin-data", "raw-data", "df_in" etc..)

Other Resources:

-   More discussions on dependencies -- https://www.tinyverse.org
-   How to name things -- https://github.com/IndrajeetPatil/second-hardest-cs-thing
-   Snapshot testing -- https://indrajeetpatil.github.io/intro-to-snapshot-testing/#/title-slide
