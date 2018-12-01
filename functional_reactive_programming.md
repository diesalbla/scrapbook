## Diary of Readings and articles. 

#### 12 June 2018

- [Conal Elliott on FRP and Denotational Semantics](https://www.haskellcast.com/episode/009-conal-elliott-on-frp-and-denotational-design). A one-hour talk, no presentations, in which Conal Elliott retails the history of how he came up with FRP (from animations). 

#### August 2nd 2018

- [Controlling Time and Space: understanding the many formulations of FRP](https://www.youtube.com/watch?v=Agu6jipKfYw). A Talk by Evan Czaplickiby, describing the basis of Functional Reactive Programming (FRP) with Elm. 

#### August 19th 2018. 

- [Implementing and Optimising Functional Reactive Programming](https://skillsmatter.com/skillscasts/9461-implementing-and-optimising-functional-reactive-programming-henrik-nilsson), a talk by Henrik Nilsson about the implementation of the [Yampa](https://wiki.haskell.org/Yampa) library. 

#### September 11th 2018.

- [Asynchronous Functional Reactive Programming for GUIs](http://dblp.org/rec/bibtex/conf/pldi/CzaplickiC13). Evan Czaplicki article introducing Elm, as a specialised variant of FRP into a discrete-only signals, push-based systems. 
- [A Farewell to FRP](http://elm-lang.org/blog/farewell-to-frp). Evan Czaplicki blog post, announcing that Elm could be based on a formulation without FRP.

#### December 1st, 2018. Functional Reactive Programming from First Principles

An article by Hudak and Wan, concerned with the key question "what does it mean for an FRP implementation to be correct". Quotes: 

> We explore the formal semantics of FRP, and how it relates to an stream-based implementation that represent (therefore approximate) continuous behaviours.
> 
> An FRP program is just a set of mutually-recursive behaviours and events, each of them built up from static (non-time varying) values and/or behaviours and vents. 
>
> A design goal for FRP is to free the programmer from presentation details by providing the ability to think in terms of "modelling". 
>
> Intuitively, a "behaviour" is a stream transformer: takes an infinite stream of sample times "t_i", and yields an infinite stream of values "b(t_i)".
>
> An implementation becomes two parts: a definition of FRP primitives, and behaviours; and a "runtime system", that interprets those behaviours by building an infinite stream of sample times and feeding it to the behavior. 



## List of references: 

In some of these names, I use FRP for the full words FRP. Some papers would shorten it in the titles, others don't. 

### Papers 

- [FRP, Refactored](https://dblp.org/rec/bibtex/conf/haskell/PerezBN16)
- [FRP from first principles](https://dblp.org/rec/bibtex/conf/pldi/WanH00)
- [Push-Pull FRP](https://dblp.org/rec/bibtex/conf/haskell/Elliott09)
- [Back to the Future. Time travel in FRP](https://dblp.org/rec/bibtex/conf/haskell/Perez17)

### Videos 
 
- [The Essence and Origins of FRP](https://www.youtube.com/watch?v=j3Q32brCUAI), by Conal Elliott. 

