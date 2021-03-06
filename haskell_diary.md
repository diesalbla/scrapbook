##### Tuesday 12th June 2018.

- [HaskellCast Episode 9 - Conal Elliott on FRP and Denotational Design](https://www.haskellcast.com/episode/009-conal-elliott-on-frp-and-denotational-design).


##### 26 July 2018

- [Simon Peyton Jones - Linear Haskell: practical linearity in a higher-order polymorphic language](https://www.youtube.com/watch?v=t0mhvd3-60Y)

##### August 2nd 2018

- [Sed, a debugging story](https://www.fpcomplete.com/blog/2018/06/sed-a-debugging-story?utm_campaign=Service%20-%20Haskell&utm_content=73275803&utm_medium=social&utm_source=linkedin)

#### Friday, November 2nd 2018

##### [ResourceT, a necessary evil](https://www.fpcomplete.com/blog/2018/10/resourcet-necessary-evil?utm_campaign=Service%20-%20Haskell&utm_content=78015420&utm_medium=social&utm_source=linkedin)

Using a small example, it starts describing a common use-case for the `ResourceT` monad transformer from `conduit`, namely,  handling resources (such as file handlers). 

> In a coroutine based system, we’re passing control of execution to some other component when we yield or await. We have no ability to install exception handlers on the actions that other component is performing

However, his main point is that, for many use-cases, the `ResourceT` is too powerful, complex, and error-prone. 

> ResourceT is an _absolutely necessary tool_ in some cases. [...] The general rule for when you need ResourceT is for dynamic resource usage [...] before you begin processing, you don’t know how many resources, or which exact resources, you’re going to need

##### [Is Rust Functional](https://www.fpcomplete.com/blog/2018/10/is-rust-functional?utm_campaign=Service%20-%20Rust&utm_content=78598434&utm_medium=social&utm_source=linkedin)

An analysis of what makes a programming language, and the style for writing programs on it, to be more or less functional; and how Rust appears under this analysis. 

##### [Lenses: compositional data access and manipulation](https://skillsmatter.com/skillscasts/4556-simon-peyton-jones)

A good and simplified introduction to lenses in Haskell. He describes the key idea of getter-setter pair, and how using type-trickery one moves from simple getter-setter types to the more generic formulations in the actual implementation. 

#### Wednesday, November 29th 2018

- [Haskellight - a Haskell framework and DSL for controlling lighting.](https://www.meetup.com/London-Haskell/events/256066832/) Control disco lights from Haskell. Peter Marks shows this system, covering both software and hardware. LED lightbulbs, electronic specifications, Arduino, chip boards designs, transistors, drivers, and a Haskell Api to progrann it.

## 2019 


- February 17th: [LambdaConf 2015 - A Practical Introduction to Haskell GADTs Richard Eisenberg](https://www.youtube.com/watch?v=6snteFntvjM). A nice explanation about what GADTs are, how they differ from normal ADTs, what the problem for type inference (lack of principal type) means, etc. 

- April 21st: [High Performance Haskell by Harendra Kumar](https://www.youtube.com/watch?v=aJvwORrBJ0o&list=WL&index=8&t=10s&pbjreload=10). Introduction to key techniques for performance optimisation in Haskell, such as function _inlining_, type-class _specialisation_, use of _strictness_, how to use efficiently use benchmarking, etc. 

- June 1st: [How we made Haskell search strings as fast as Rust](https://tech.channable.com/posts/2019-03-13-how-we-made-haskell-search-strings-as-fast-as-rust.html).

- 
