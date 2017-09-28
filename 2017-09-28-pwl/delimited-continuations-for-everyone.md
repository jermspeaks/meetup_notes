# Delimited Continuations for Everyone

Have you thought of continuations as something that only program semanticists and compiler implementers are concerned with? In fact, the concept of continuations appears everywhere and is useful for everyone. In this talk, Kenichi will introduce delimited continuations from the programmer's perspective directly without requiring any program transformation or semantic arguments. He will then show how various and seemingly complex programs can be written simply and concisely by manipulating delimited continuations. The goal here is to convince you that delimited continuations are useful in day-to-day programming. Finally, Kenichi will speculate on the Curry-Howard isomorphism of delimited continuations, which could open the door for the introduction of delimited continuations into theorem proving.

## References

Representing Control: A Study of CPS transformation by O. Danvy and A. Filinski (Introduction to delimited continuations)
Abstracting Control by O. Danvy and A. Filinski
Functional Unparsing by O. Danvy
The Theory and Practice of First-Class Prompts by Matthias Felleisen
A Formulae-as-Types Notion of Control by T. Griffin
Cogen in Six Lines by P. Thiemann
Representing Monads by A. Filinski

## Biography

Kenichi Asai is an associate professor in the Department of Information Science at Ochanomizu University, Japan. His research interest centers around the "essence" (in his own way) of programming languages. He designed a Scheme-based reflective language Black (code), because reflective languages represent the essence of interpreters in the most distilled way. He studied partial evaluation because it is the only general framework for compilation of reflective languages. He was attracted to delimited continuations because they explain various complex behavior of programming languages in a succinct and understandable manner. He is also interested in education of programming languages, because teaching forces us to think about the essence. He is a strong advocator of Design Recipe, which he believes is one of the essence of programming in general, and uses it to teach OCaml in the university. He ported the universe teachpack of Racket to OCaml, because it exhibits the essential model of game programming.

Recently, he is co-developing an interactive OCaml type debugger as well as an OCaml stepper that uses delimited continuations in a non-trivial way. He believes both the tools are essential for beginning students.
