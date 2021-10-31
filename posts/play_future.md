
# On the future of Play Framework

### On the future of the Play Framework (Jonas Boner, 20th of October 2021, Lightbend Blog)

[Jonas Boner, on the Lightbend Blog](https://www.lightbend.com/blog/on-the-future-of-play-framework)

TL;DR - We are working to form a community-led organization that would take responsibility for the future development of Play Framework outside of Lightbend.

Ever since I started Lightbend (formerly known as Typesafe) with Martin Odersky, now more than 10 years ago, Open Source Software (OSS) has been at the heart of what we do. It is fair to say that Lightbend would not exist without the transforming power of OSS and the amazing communities around our products Scala, Akka, Play, and more.

Building software in the open, putting your work out there for everyone to see and judge can be scary, at least initially, but can also be so rewarding. OSS is the perfect environment to try out crazy ideas, to try to reach a bit higher, and to be able to do it with peers that share the same passion and joy for programming, curiosity, creativity, and urge for change, regardless of background, gender, citizenship, ethnicity, political values, or whatever. When it works it’s magic. I am personally so grateful for OSS and what it has enabled me to do, learn, and experience, and the long-lasting friendships it has helped me build.

Lightbend started around a vision to build the best possible OSS development platform and tools for the emerging Cloud (multicore and distributed systems), specifically targeting microservices, web applications, and streaming data systems. On this quest, which started with Akka and Scala, we added the Play Web Framework, which—being built on top of Akka with a strong async and non-blocking story—was a great and natural addition to the stack.

Play quickly grew to become one of the most loved and used web frameworks for full-stack applications in Java and Scala, with a large and passionate developer community. It has played a key role in bringing the Reactive Principles to web development and has pushed the envelope for web frameworks when it comes to the overall developer experience. Over the years Play has played an important role in Lightbend’s overall strategy as a core part of the Akka Platform (formerly known as Lightbend Reactive Platform) and is very much loved by our customers allowing them to build full-stack applications in a Reactive way, from top to bottom.

However, as a majority of our customers and the industry at large have moved to the Cloud, we have steered our focus more and more towards our core competency, our DNA, the reason why we started this company: building the best developer platform and experience for distributed systems, the Cloud, and the emerging Edge ecosystem. That means primarily focusing on Akka Open Source, and our new PaaS-platform Akka Serverless, a product that enables the values of Akka—low-latency and high-throughput real-time data, paired with incredibly high levels of scalability, reliability, and availability—to any developer, packaged up a serverless, simple, and to a large extent declarative developer experience, regardless of the language they want to program in.

All this means that we as a company are still as passionate about OSS as ever, but will not be able to be the stewards and main developers of the Play project anymore. This does not mean that Play is dead and that you should migrate off it. Play is rock-solid and used by hundreds of thousands of Java and Scala developers every month. Play is still extremely relevant to today’s application and web development and has a passionate and very capable community around it ensuring that it has many good years left.

We at Lightbend have simply finished writing our chapter in the story and are now trusting the following chapters to the community and power of OSS. If you love Play and care about its future then step in and help out. It is, as I said, both extremely rewarding and fun.

Together with contributors in the Play community, we intend to form a community-led organization that would take responsibility for the future development of Play outside of Lightbend. This will only be possible if we gather Sponsors that are willing to donate money on a monthly basis, and Contributors that can put work into the Play codebase and the administration of the project. We’ll most likely form a Steering Committee for Play where Sponsors and Contributors can collaborate to form Play’s future.

If you as an individual, or your employer as a company, are willing to contribute to this journey, please reach out to us at play-team@lightbend.com.

Tell us how you want to be part of it.

Play needs you.


### Matthias Kurz (Oct 21 2021)

[Comment on Lightbend Discuss](https://discuss.lightbend.com/t/on-the-future-of-play-framework/8920/2)

Hi everyone!

Some of you who followed the Play GitHub repository 22 and this user forum in the last few years may know me 13.
Since I was the most active Play contributor in the last years and, in the last 1,5+ years, probably the last core contributor left who actually worked on Play on a regular basis, doing most of the work to make the last releases even happen, I finally want to comment on the current situation and what we have planned with the future of Play.

First of all, let me clarify one thing: I never worked for Lightbend and never received one single cent for my work on the framework and its ecosystem. I want to mention this because it happened to me more than once already that people thought I work for Lightbend, because of the amount of work I did for the framework in the last 7 years. Basically, I am just a random guy on the Internet who invested a lot of time since 2014 to push Play forward by adding new features and fixing bugs (until I even became #1 contributor just recently 13, based on commits) and helping the community to solve their problems. Plus making sure the build runs stable ;) (BTW: I already used Play 1 as well already since 2010, contributing code to it too). So, in the last 1,5+ years Lightbend retreated more and more from Play, which meant there was hardly any of them working actively on the framework anymore on a regular basis, like it used to be. For me that meant the work I was doing to keep Play alive was getting even more and more, almost impossible to handle for me next to other projects I was working on to pay my bills and next to my family.

Now, as you have read the blog post, Lightbend is working with me and some other people “to form a community-led organization that would take responsibility for the future development of Play Framework (outside of Lightbend)”.

#### So, what does that actually mean?

[...] We are planning to move Play to https://opencollective.com/ - a place where people and organizations can sponsor an Open source project with recurring or one-time donations in the (IMHO) most transparent way possible. That means that people like me, who really deeply cared (and still care) about Play in the last years are able to continue their work on the framework, while also finally getting paid for their time invested - getting paid from organizations and individuals like YOU, people and companies that use Play on a daily basis, that rely on Play, that run Play applications in production to thrive their business and that profit from the work that people like me, passionate Open source contributors, do in their free time to keep a fantastic framework alive and to even push it further.

In the last 6 month, when it dawned to me that Play would basically be (or become) unmaintained if I wouldn’t be motivated to contribute, I was thinking a lot about what to do with Play and how I should personally stay involved with [it]. Not just once I was thinking to just open a GitHub sponsors account. However, in my opinion with a fully transparent platform like Open Collective we finally found the best solution. For me, moving Play to Open Collective just feels right to me, I think it is the right thing to do for Play, its users, its community and everybody else who is interested in the success of the framework. From the perspective of a passionate Open Source developer, I think it’s the absolutely best solution for everyone involved. IMHO Play should be run by the community. Not by an individual, not by a single company, but by people who really care about the framework.
And people who contribute to Play should get paid accordingly by the companies who profit from their work.

I have seen from other projects (like https://opencollective.com/socketio 25, https://opencollective.com/webpack 11 or https://opencollective.com/generator-jhipster 7) that it is possible to build a healthy, stable and fair relationship between contributors and sponsors, where people and companies who are interested in the success of a project can support the project by giving money, which will be used to pay contributors, like me, for the work they are doing - be it part time, be full time or just for implementing specific features.
I don’t think I have to prove to anyone that for me working on Play was never about making money and that money was absolutely never my motivation (and of course no one ever forced me to contribute or to give those talks at user group meetups, I just wanted to help to create a great piece of software ;). But now that Lightbend quits and wants to hand over Play to someone else, things already have and also need to change.

So to everyone that wants to keep the framework alive; to every company out there that is invested into and depend on Play; to everyone that has Play applications running in production; basically to everyone that has an interest in the success of Play and that the project prospers:
If you are interested that there is someone that cares about the project (and related sub-projects), maintains it and pushes it forward, please sponsor me and other contributors! You will not invest into me or other contributors as individuals, you will not invest into a company, but you will invest into the project and its community.
We are planning to open the Open Collective account soon, so please let us know by contacting us via the e-mail address mentioned in the blog post or by sharing your thoughts by commenting below in this thread if you or the companies you are working for are willing to participate. Of course if you have any questions, please let me and us know, I am looking forward to interesting conversations.

Thank you very much!

Matthias

PS: I know this post is solely about funding and money. Of course we are super happy if people and organizations want to invest time to write code for Play and contribute and maybe even become maintainers. However, what I think is important right now is to collect money so we can keep going as soon as possible.
