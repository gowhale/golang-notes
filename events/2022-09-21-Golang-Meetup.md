# Golang MeetUp
Date: 21/09/2022
Location: Monzo Bank, London

Talks: 
- Talha Altinel - Bundling Tasks with Task File
- Paul Jolly - Go + CUE - a match made in heaven
- Angad Nadkarni - Performance from First Principles

## Bundling Tasks with Task File
Talha Altinel gave a great talk about Task Files and their use. It was great to see how tasks can be bundled in task files and combine different processes like running go tests and linters.



## Go + CUE - a match made in heaven
Paul Jolly shared knowledge about CUE and gave a live demo. In short, I saw that CUE files can be generated to create a configuration file. This file can be validated by a CUE schema ensuring that configuration variables are of the right type. This is super helpful in Go as often engineers will be casting a JSON or YAML configuration file into a struct. If this config file has already been validated by CUE then the struct will have values that we expect. 

“CUE is an open-source data validation language and inference engine with its roots in logic programming. Although the language is not a general-purpose programming language, it has many applications, such as data validation, data templating, configuration, querying, code generation and even scripting. The inference engine can be used to validate data in code or to include it as part of a code generation pipeline.

A key thing that sets CUE apart from its peer languages is that it merges types and values into a single concept. Whereas in most languages types and values are strictly distinct, CUE orders them in a single hierarchy (a lattice, to be precise). This is a very powerful concept that allows CUE to do many fancy things. It also simplifies matters. For instance, there is no need for generics and enums, sum types and null coalescing are all the same thing.” - https://cuelang.org/docs/about/ 

Key takeaways:
I plan on using CUE in my personal project: https://github.com/gowhale/go-shopping-list to get hands-on experience with CUE and gain a deeper understanding of CUE benefits.

Links:
https://cuelang.org/docs/integrations/go/ 



## Performance from First Principles
Angad Nadkarni demonstrated extreme optimisation of their code. 

<img width="1245" alt="image" src="https://user-images.githubusercontent.com/32711718/192785102-af9b5124-dc92-46d5-82fd-0e3a55e69dc3.png">

Screenshot taken from: https://www.youtube.com/watch?v=-NW7Z-JHOIA 

As you can see from the above screenshot you can see how in the talk Angad takes us through the process of being able to handle 50K cells to 150 million cells.
