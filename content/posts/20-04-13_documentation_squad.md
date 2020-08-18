+++
title = "Documentation: Squad"
date = 2020-04-13
author = "fmendes6"
draft = false
+++

*_This is part 2 of 3 about feature documentation on feature-based teams._*

[Part 1 - The problem](/posts/20-04-06_documentation_problem)  
**Part 2 - Squad level documentation**  
[Part 3 - Chapter level documentation](/posts/20-04-20_documentation_chapter)  

As mentioned before, one of the main problems between different squads is the creation of silos, which typically results in people knowing very little about the other features that exist in the product.

To help solve this problem, I believe squads should have a central point of information, as well as a way for them to expose and communicate what their feature is about to other teams. 

This means a document that is:
* Short and to the point;
* Understandable by everyone on the squad (engineers, designers, testers and project managers)
* High-level with no platform-specific implementation details. For example, as an android developer, I don’t want to read iOS-specific tracking considerations in this document.

With these considerations in mind, some of the use cases I envision for this document would be the following:

> As an Android developer, I want to know what my Android colleagues are working on and how to use the feature.    

> As a team lead, I want to know what is the roadmap of the teams I am leading (or others) during a meeting, as well as, how the data is flowing between platforms.    

For these scenarios and considerations, I have come up with the following document structure and a template ([see here](https://gist.github.com/fmendes6/51961e330f1766e5f4020de4e27a5d3e)) that I use:

1. **Usage** - Step by step on how to use the feature.
2. **Use cases** - The main use cases of the feature and what actions can the user perform.
3. **Roadmap** - Which release version was the feature first included in.
4. **Team** - Who worked on the feature.
5. **Architecture overview** - A brief overview of the data flow, how it is architected at a very high level.
6. **Strategies**
		1. Tracking
		2. Localisation
		3. Content
7. **Resources** - With links to other documents and platforms.

Keep in mind that this template is merely a guideline, so make sure you adapt it to your context.

Finally, I would advise you to avoid including any temporary solutions or information regarding the current state while the feature is still in development, as that would increase the probability of the document becoming outdated. 