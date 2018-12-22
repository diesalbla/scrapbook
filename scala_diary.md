
### 2018

#### June

##### Sunday, 10th of June 2018.

- [Speeding up Compilation Time With `Scalac-Profiling](https://www.scala-lang.org/blog/2018/06/04/scalac-profiling.html)
- [Advanced Tagless Final](https://www.youtube.com/watch?v=E9iRYNuTIYA&t=1007s-)
- [Scalaz 8: A whole new game (John A. De Goes)](https://www.youtube.com/watch?v=sFGnFKMSmL0)


##### Wednesday 13th June 2018.

- [Scala Blog - News on Scala Collections](https://www.scala-lang.org/blog/2018/06/13/scala-213-collections.html)
- [Scalaz 8 IO vs Akka (typed) actors vs Monix (part 1)](https://blog.softwaremill.com/scalaz-8-io-vs-akka-typed-actors-vs-monix-part-1-5672657169e1)

##### Monday 18th June 2018.

- [Cancelable IO – Alexandru Nedelcu](https://www.youtube.com/watch?v=UeyGHhYJqG4). A Talk from the Typelevel Summit, satellite to ScalaDays-EU, May 2018. 
  Discusses concurrency in `scala.concurrent`, the developments of [`monix`](https://github.com/monix/monix), and the inception of [`cats-effect`](https://github.com/typelevel/cats-effect).


##### Sunday, July 1st 2018.
 
- [SF Scala, Rolando Manrique, fs2-blobstore Store implementations and use cases](https://www.youtube.com/watch?v=xM3N4hAQMFs)


##### Sunday, July 2nd 2018. 

- [Constraints Liberate, Liberties Constrain — Runar Bjarnason](https://www.youtube.com/watch?v=GqmsQeSzMdw) 


##### Saturday, July 14th 2018. 

- [Inference Driven Design](https://mpilquist.github.io/blog/2018/07/04/fs2/) Describes how the design of the `fs2` trait was constrained by the Scala compiler type inference limitations. 
- [Avoiding Microservices Mega-disasters](https://www.youtube.com/watch?v=gfh-VCTwMw8&t=10s). 


##### Sunday, July 22nd 2018. 

- [Supervision and Error Handling in ZIO, `akka`, and `monix`](https://blog.softwaremill.com/supervision-error-handling-in-zio-akka-and-monix-part-3-series-summary-abe75f964c2a). Describes some technical differences between `ZIO` and `monix.Task`. 

##### Thursday, July 26th 2018. 

- **Rage against the System**, talk by Jon Pretty at [Meetup](https://www.meetup.com/Scala-in-the-City/events/251790948/). 

##### Wednesday, 1st August 2018. 

- [Pull Push: Please stop polluting our imperative languages with pure concepts](https://www.youtube.com/watch?v=449j7oKQVkc), a talk by Ron Pressler at the CurryOn conference, on July 2015, about the abuse of Monads on imperative languages. 
  The talk has an accompanying [blog post](http://blog.paralleluniverse.co/2015/08/07/scoped-continuations/). 



##### Wednesday, 1st August 2018. 

- [Optimising Tagless Final (Part 2)](https://typelevel.org/blog/2018/06/27/optimizing-tagless-final-2.html). 


##### Sunday, September 2nd 2018.
- [Http4s error handling with Cats Meow MTL](https://typelevel.org/blog/2018/08/25/http4s-error-handling-mtl.html).


##### Monday 17th September 2018.
- [SF Scala: Seth Tisue, Scala Compiler Plugins 101](https://www.youtube.com/watch?v=Dt_AIFNQuWc), 

#### Saturday, October 13th 2018.
- [Speed Up things in Scalac and SBT](https://kubuszok.com/2018/speed-up-things-in-scalac-and-sbt/). A list of detailed tricks for improving CI builds in Scala projects. Reared towards backend development (an application exposing an API and working against a Database). 

#### Tuesday, November 7th 2018. 

- [Monix: Task’s Bracket, Resource[F, A] and Streaming](https://vimeo.com/299313903) Alex introduces the use of Monix primitives for `Resource`, `bracket`, and the streaming type `Iterant`.

#### Sunday, November 11th 2018

- [A Tale of two Monix Streams, Scala Days 2018](https://monix.io/presentations/). Alex describes main abstractions of Monix, and introduces them with the intuition of Scala collections with laziness and effects. He contrasts `Observable`, for push-based streaming, with `Iterant`, used for pull-based streaming. 
> Architecture is frozen music. Data structures are frozen algorithms. Freeze Algorithm into a Data Structure.


#### Wednesday, November 29th 2018.

- [Scala Italy 2018 - Fabio Labella - Shared state in pure FP: when a state monad won’t do](https://vimeo.com/294736344)

#### Saturday, December 22nd 2018.

- [Blazing Fast, Pure Effects without Monads](https://www.youtube.com/watch?v=L8AEj6IRNEE). Talk by Jon de Goes, about Scalaz using Kleisli Arrows. It describes the use of arrow operators for IO operations. 


### 2019

- 25th February: [The Death of FInal Tagless](https://skillsmatter.com/skillscasts/13247-scala-matters), on-site. Jon discusses the Tagless Final style in its full expression: capabilities as type-classes, type-classes as traits and implicits, and algebras as trait parameterised on a higuer-kind type parameter. 

- 17th March: [SF Scala: Bill Venners, Property-based Testing in ScalaTest 3.1](https://www.youtube.com/watch?v=lKtg-CDVDsI), a talk about the new property-testing capabilities of ScalaTest. 

- 25th March: [How I Rebuilt the Typelevel Ecosystem with Fury](https://skillsmatter.com/skillscasts/13245-scala-matters). Talk attended on-site. 

- 25th April: [Adam Warski - Descriptions, APIs and Tapirs](https://www.youtube.com/watch?v=TARW95QDdew), attended on-site. Adam describes Tapir, a library for purely-functional description of APIs. The goal of the library is to describe the API as an OpenAPI spec would.

- May 20th: [The Elements of Tagless Final Style](https://skillsmatter.com/skillscasts/13253-scala-matters). Noel Welsh presents the Tagless-Final style in its essential form, using the classical calculator-like example.


#### Sunday, May 26th 2019.

- [Networks and Types — the Future of Akka by Konrad ‘ktoso’ Malawski](https://www.youtube.com/watch?v=Qb9Cnii-34c).

- [6 reasons why not to use Akka Cluster for interservice communication in a microservice architecture](https://blog.softwaremill.com/6-reasons-why-not-to-use-akka-cluster-for-interservice-communication-in-a-microservice-architecture-2736d5223573). 

- [Tutorial 1 - Customized `parTraverse` using `Deferred`](https://www.youtube.com/watch?v=uuocHqdnoS0&t=601s). 
- [Tutorial 2 - Sharding a stream of values using Fs2](https://www.youtube.com/watch?v=FWYXqYQWAc0)
