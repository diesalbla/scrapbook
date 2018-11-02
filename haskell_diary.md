##### Tuesday 12th June 2018.

- [HaskellCast Episode 9 - Conal Elliott on FRP and Denotational Design](https://www.haskellcast.com/episode/009-conal-elliott-on-frp-and-denotational-design).


##### 26 July 2018

- [Simon Peyton Jones - Linear Haskell: practical linearity in a higher-order polymorphic language](https://www.youtube.com/watch?v=t0mhvd3-60Y)

##### August 2nd 2018

- [Sed, a debugging story](https://www.fpcomplete.com/blog/2018/06/sed-a-debugging-story?utm_campaign=Service%20-%20Haskell&utm_content=73275803&utm_medium=social&utm_source=linkedin)

##### Friday, November 2nd 2018

- [ResourceT, a necessary evil](https://www.fpcomplete.com/blog/2018/10/resourcet-necessary-evil?utm_campaign=Service%20-%20Haskell&utm_content=78015420&utm_medium=social&utm_source=linkedin). Using a small example, it starts describing a common use-case for the `ResourceT` monad transformer from `conduit`, namely,  handling resources (such as file handlers). 
> In a coroutine based system, we’re passing control of execution to some other component when we yield or await. We have no ability to install exception handlers on the actions that other component is performing

However, his main point is that, for many use-cases, the `ResourceT` is too powerful, complex, and error-prone. 

> ResourceT is an _absolutely necessary tool_ in some cases. [...] The general rule for when you need ResourceT is for dynamic resource usage [...] before you begin processing, you don’t know how many resources, or which exact resources, you’re going to need
