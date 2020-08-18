+++
title = "A documentation problem"
date = 2020-04-06
author = "fmendes6"
draft = false
+++

_This is part 1 of 3 about feature documentation on feature-based teams._

**Part 1 - The problem**  
[Part 2 - Squad level documentation](/posts/20-04-13_documentation_squad)  
[Part 3 - Chapter level documentation](/posts/20-04-20_documentation_chapter)  

In an attempt to improve its teams' autonomy, Spotify adopted an [engineering culture](https://www.youtube.com/watch?v=4GK1NDTWbkY&list=RD4GK1NDTWbkY&start_radio=1&t=4) that would allow small cross-functional teams to have end-to-end responsibility for the stuff they build, from design, commit, deploy, maintenance to operations.

Instead of a model where teams are organised by the platform that they work on, the "Spotify model" proposes teams to be split by feature, with each team, now called a squad, having one or two representatives of each competency (Product, Android, etc.).

| Feature 1 | Feature 2 | Feature 3 | 
| ------ | ----------- | ----------- |
|  _Product_ | _Product_ | _Product_ |
|  _Android_ | _Android_ | _Android_ |
|  _Web_     | _Web_     | _Web_     |
|  _Backend_ | _Backend_ | _Backend_ |
|  _QA_      | _QA_      | _QA_      |

This organisation enables cross-functional squads to focus on a particular domain problem that they call a mission, and nothing else. This focus naturally leads to faster delivery since all implementation decisions are now taken locally but comes with the cost of further increasing information silos between squads if communication isn't promoted and consistent, which usually results in:

- People knowing very little about other features. With different features under development in parallel, it becomes hard to keep track of what is done and how.
- Joining another squad is almost like joining a new company. You might share (or not) the same codebase, but the domain and the problem you are tackling can be completely different, which is excellent for people that want to work on something new from time to time but it is also costly for the company since it can take a considerable amount of time for someone to become productive.

Teams following this culture will take advantage of the physical proximity and faster (cross-platform) communication, which leads to quicker development but will lose out on cross-squad debate that leads to more sound and thoughtful decisions, consistent and long-lasting knowledge across the company. 

To tackle this problem, engineering teams promote code reviews from other squads in an attempt to reduce the creation of silos, but in reality, this generally results in reviews that do not consider the context and the overall high-level solution behind a code change, as engineers will mostly evaluate/review the technical aspects and not so much the global solution. To make matters worse, some squads will opt to review only squad-related work so that they can speed-up squad delivery but that further increases the existing silos of information between squads.

These problems lead me to believe that companies need to seriously consider taking the time to communicate between squads because a company that favours communication before development and sharing information afterwards, will be able to:

- Reuse some of the systems, platforms or tools that were developed by different squads instead of creating new ones, avoiding the cost of twice the developing time.
- Reuse systems that were developed in the past instead of relying on specific individuals. Those individuals might have created a great product at that time, but the engineers of today do not have the time to learn how to use it or are in place to reuse it.
- Share existing knowledge of the systems that are in place with any new hires, or even when moving people from a different squad. Without proper documentation and communication processes, a recent hire will not know about what is being developed in the other ten squads, why and how.
- Keep a record of the context and considerations at a particular time, so that squads can take quicker and more thoughtful decisions in the future.
- Have squads that provide more accurate estimates of pieces of work that were already developed by others.

Full autonomy is a problem when squads start developing tools that other squads already developed or when they decide to implement solutions that negatively impact other teams. It sounds great, but just like any organism, a product is not merely the sum of its parts. If our digestive system does not process food properly, there will be an impact on all the other organs.

And here, those "boring" and "slow" processes that "are in the way" come into play and save a lot of the company's time and money.

However, discussing ideas and solutions sounds great, but different squads are usually at different stages of development so they might not have the time or the willingness to have meetings and calls to approve someone else's work.

So instead of having synchronous communication across squads/chapters, each squad should be responsible for communicating about what it is developing, how and why in one-way asynchronous communication. This opens up the possibility for outside feedback, which might come or not, but at least valuable information is saved for future reference.

With this in mind, the next blogposts in this series will propose two new types of documentation, one product-oriented for sharing between squads and one competency-specific for sharing between the chapter.