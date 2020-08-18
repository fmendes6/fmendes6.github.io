+++
title = "Documentation: Chapter"
date = 2020-04-20
author = "fmendes6"
draft = false
+++

_This is part 3 of 3 about feature documentation on feature-based teams._

[Part 1 - The problem](/posts/20-04-06_documentation_problem)  
[Part 2 - Squad level documentation](/posts/20-04-13_documentation_squad)  
**Part 3 - Chapter level documentation**  

All platforms are different and deal with different limitations/constraints so is considerably harder to create a template the would work for all platforms. However, one question that we should always have in mind is: 

_” What would a colleague of mine need to know if he/she started to work alongside me in a shared codebase?”_

This helps us envision the use case in which a document would be useful:

> As an iOS developer, when I join a new squad, I want to have a high-level idea of how my iOS colleagues have implemented the feature and how all the components interact with each other.   

For this scenario, I have come up with a template ([see here](https://gist.github.com/fmendes6/96f2ebfb190b4aa522f660059f3d918d)) that would work well for most features, independently of the feature that we implement:

1. An overview of the architecture and services used;
2. How it interacts with other parts of the app;
3. A description of critical operations; 
4. Testing considerations;
5. FAQ with common questions;
6. References to documents and pages specific to the platform.

Finally, I would advise you to avoid any code snippets (use pseudo-code instead) and as fewer implementation details as possible, as these should live closer to the code in the pull requests description.

Once you finish writing the document, I would recommend you to request a review from your peers and improve it until they answer affirmatively to the following question:

_”If I just started working on this feature and I looked at this document, is the content here enough for me to start without having to reach out to the original developers?”_