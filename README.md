# jovial
Keep dependency issues in Jupyter notebooks at bay with Docker (and soon, Compose)

#### NB: Work in progress!

The tool is still missing most of its features, and core functionality may be subject to change at any time.

## What is this, and what is it for?
TL;DR: a quick-fix for the inter-faculty rivalry between Informatics and Mathematics

In academia, researchers often use Jupyter notebooks for quick, "throwaway" code in their analyses and experiments.
This leads to notebooks leaning on countless dependencies and/or only capable of working with very specific environments (the perennial "it works on my machine" problem).
For code that only needs to work once on one machine, this is a non-issue - however, it makes maintaining, reproducing or repurposing the code unnecessarily difficult.

*writer's block, will expand upon this later*

- Version reqs for deps drift apart over time
- May be pertinent to update parts of the code without being stuck with the old version for other parts, e.g. one component needs a dependency for a newer API while another uses a numerical analysis tool which was last updated in the late Paleozoic
- Solution? Isolate and containerise components as Docker microservices, and stitch it together with Compose
