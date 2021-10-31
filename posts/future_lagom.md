

## The future of Lagom: 



### Jeremy Pollock. 

Our guidance to developers out there is that they should begin any new development using either Akka Platform or Akka Serverless. There is no new feature development planned currently for Lagom. Many of our customers enjoyed Lagom in the early days but began to run into too many blockers from all of the framework constraints, e.g. single DB type support.

Last year, we released many features around microservices development in the Akka Platform that made it functionally equivalent to Lagom. We also put out a documentation guide that demonstrated how to do service APIs and event sourcing/CQRS in Akka Platform (Akka Platform Guide :: Akka Platform Guide 12).

We are supporting Lagom customers far into the future and this includes bug fixes, technology updates and security patches. We may add functionality at some point but right now, all engineering focus is on Akka Platform and Akka Serverless, both of which encompass what Lagom was doing and are better platforms for evolving the ideas and capabilities.

From a project perspective, Lagom is very different from Play, given that Lagom has never received much community support as compared to Play. Many of our Lightbend customers have used Lagom successfully and still do. We just haven’t seen the adoption and community engagement on the Open Source side of things to warrant pursuing a path that we’ve begun with the Play Framework.

To sum things up:
    
    
- Lagom will not continue to evolve and have new features added
- Lightbend will support our customers using Lagom for the foreseeable future
- Lagom is not going anywhere, and can still be used by any developer
- We recommend people base new projects, and if needed migrate existing projects, to the new microservices support in Akka Platform or leverage Akka Serverless


### James Roper: (Oct 29 2021)


Allow me to also add to this (I was one of the original creators of Lagom).

When we created Lagom, we had Akka, which was a powerful toolkit for distributed computing, and we had Play, which was an high productivity framework for web development focused on developer experience. There was an obvious gap in this at the time - a high productivity framework for distributed computing focused on developer experience. At the time, microservices were also all the rage, and while Play was ideal for web development, it was missing a lot of features needed for building reactive microservices - for that you had to fallback to Akka, which was more toolkit-like, gave you all the power, but not such a good developer experience, no clear guidance on how to do things.

So, we knew we needed something to fill this gap. We had three options, extend Play’s functionality, extend Akka’s functionality, or create something new that combined them both. For better or worse, and we decided to ride the microservice wave and create an entirely new framework for building microservices, based on Play with the same focus on productivity and developer experience that Play had, while leveraging Akka to provide the distributed computing and reactive principles that we believe are the foundation of a microservice architecture.

Lagom was born. Over the next few years, a few things happened.

**Akka typed was in development**, and this provided an opportunity to create new, more opinionated and more developer experience focused APIs in Akka itself around things like event sourcing, cluster sharding and projections. In that instance, Lagom had been an excellent proving ground for strongly typed APIs on event sourcing, and it was from this experience that akka-persistence-typed was built, as well as akka-projections and akka-cluster-typed. Alpakka also began to fill a role that some of the Lagom APIs offered. We started encouraging people to use these new more powerful, complete and widely compatible APIs that were even nicer than Lagom’s APIs given the experience we had learnt from developing Lagom itself.

**gRPC became a thing((. If you look at a Lagom service descriptor, and the capabilities there, and a gRPC descriptor, you’ll notice, they map almost perfectly 1:1. Both support unary, server streamed, client streamed and two way streamed calls. Both share the idea of a service with named calls. Both have the concept of a single (possibly streamed) input and output message. Their main difference was in implementation, gRPC was an entirely new protocol, Lagom service descriptors mapped down onto REST and websockets for streaming. When gRPC came around, I actually prototyped a gRPC based implementation of Lagoms services, it just worked, it was a clean mapping of features. We had also, for a long time, wanted to offer the option of rather than specifying the interfaces in code, specifying them in something like OpenAPI, and generating the code. gRPC gave us that for free, which also brought a much stronger polyglot story. In the end, we thought, why invest further in the Lagom service API, when we have gRPC that does exactly what we’ve always wanted. We instead created akka-grpc, and started pointing people towards that.

**Kubernetes became a thing**. The part of the Lagom story that we never quite got around to answering the way we wanted was the production story. We did deliver something called ConductR, but it never really took off, in part due to it being our own proprietary offering, when at the same time Kubernetes was rapidly becoming popular. Kubernetes offered the production experience we wanted Lagom to have, but it didn’t need Lagom, you could run Play and/or Akka apps just fine on Kubernetes, we didn’t need any special developer support like Lagom was able to provide. We started encouraging people to use Kubernetes with the Kubernetes support we had created for Akka cluster.

I think the biggest feature of Lagom that I like that hasn’t quite been solved is the development runtime - Lagom let’s you start a whole system worth of services, all able to hot reload the moment you change a file, with a single command, and you get this out of the box with no configuration or scripts or anything that you have to maintain. In some cases, this feature alone probably makes using Lagom still worthwhile today. But it’s not enough of a compelling feature for us to justify continuing the development of the whole framework. Plus, there are ways to achieve a similar thing with both Maven and sbt, albeit with a fair bit more manual configuration and/or scripts that need to be written.

So that’s a brief history of Lagom, and explains how we got to where we are today. I think Lagom played a key part in the evolution of our offerings at Lightbend, and what we set out to achieve with Lagom has largely been successful, in filling that gap between Play and Akka, both from our own efforts and in concurrent industry efforts that superseded our own.

So, my thoughts on the future of Lagom is that almost everything you can do with Lagom today, you can do with more developer friendly and powerful technologies that have largely made Lagom redundant. As Jeremy said, we’re going to continue supporting Lagom for the foreseeable future, for those that want Lagom - there is a better path forward than using Lagom itself.


### Kyle Florence (Oct 29 2021 5:20)

James: thanks for the additional information. Your description matches exactly what I had seen while working in the Lightbend ecosystem, so I totally understand the shift away from Lagom.

I did want to add my appreciation for what Lagom offered, which was an opinionated and clear way to develop distributed systems that supported both API and message interfaces. Our company had already been using Play for years, and we had dabbled a bit in Akka as well, but without Lagom our choices would have been to either roll our own framework on top of something like Akka/Play, switch to a different ecosystem entirely, something like Spring Boot, or change our development paradigm all together by trying to figure out how to move our existing processes into a serverless environment. Because we are a fairly small shop without enough resources to really take on something like the latter point, and because we wanted to stick with Scala, Lagom made it easy for us to make the jump into distributed systems.

I think our first service integration was in 2018, although we had initially considered Lagom all the way back in its inception in 2016, but at the time Scala was not yet supported. It was overall a great experience as it caused us to re-think about how we design and develop our services. It was our first time with true event sourcing and CQRS and also our first time integrating our services with Kafka, Kubernetes and Akka Cluster. However, we also quickly found pain points, as the design of Lagom was intentionally restrictive in many ways, and unfortunately by the time we really had a handful of services developed and deployed, development against Lagom was already slowing.

But as you said, just as Lagom was a stepping stone for Lightbend, it will also be a stepping stone for us. Lagom had provided the guard rails we needed for our first foray into distributed systems and many new and useful design paradigms, and we now posses a lot of knowledge which we can apply to the next generation of services we build. Our intent was always to standardize around one framework which would meet our general business needs in order to create a more consistent developer experience and reduce overhead and complexity, while also designing our processes around the expectation that we will eventually support a more diverse set of polyglot services. We have not yet tried out the Akka Cloud Platform or Akka Serverless, but at least from what I’ve read a lot of the concepts will carry over.

PS: If I could go back in time, I’d probably try to generalize some of our conventions libraries (think: cross-cutting concerns like auth, testing patterns, exception handling, etc) at the Akka level instead of the Lagom level, work that will now become a higher priority. Even while we were developing those, we already knew scoping them to Lagom was short-sighted, but as you probably know it takes a lot more time and cognitive overhead to generalize things at a higher level, and so we ended up scoping a lot of them just to Lagom. This, in combination with establishing new developer workflows, will probably be the biggest hurdle for us to overcome when moving on to a new system.
