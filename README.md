# Maintaining Direct File's Fact Graph

This branch preserves an open-source computer-readable representation of the tax code.

## Goals

For now, as an all-volunteer effort, the goal is simply to keep the tax scope covered by 
[Direct File](https://directfile.irs.gov) accurate through the 2025 tax year. Perhaps we do more, and that'd be great. But the tax code and forms change around every year, and step 1 is just to keep up with all that churn.

If that goal doesn't sound ambitious enough for you, think about what this could make possible:

- Tools that allow anyone to check to see if their own tax provider gave them all of the credits they were entitled to and file for any credits that were missed. Or to help the millions of people who don't file taxes easily discover that they have a tax refund waiting for them.
- States develop their own tax filing tools that support both state + local taxes
- When the Federal government gets their act together, Direct File can be rebuilt faster, cover more people, and let most Americans file their taxes for free.

## Where this might go (if there's a lot of volunteer interest)

Anything that improves the representation of the tax code through the fact graph is fair game:

- Making it easier to develop the fact graph
  - Simplifying the code base
  - Adding CI + testing
- Adding any tax scope above + beyond what was covered by Direct File, **so long as it's verifiably accurate** 
- Maintaining any tools that help verify the correctness of the fact graph (potentially including the frontend, PDF generation, and the Flamingo Fact Checker)

## What we're not doing

- Anything that takes more time and energy than a zero-budget volunteer effort can support
- Attempting to maintain Direct File as a whole, or building any of the spin-off tools mentioned above. Those are all great ideas, but this is not the place to work on them. The hope is that some of those more-ambitious projects will spin up, and all of them can use this shared, public representation of the tax code.

## Can I help?

**Heck yeah!** Volunteers are welcome. Be kind and patient and we'll get along just fine. Check out [ONBOARDING.md](/ONBOARDING.md) if you want to help out.

## Background and Acknowledgements

This code stands on the shoulders of giants, born from the open-sourced [Direct File](https://github.com/IRS-Public/direct-file). Those giants included team members from the [IRS](https://www.irs.gov/), [USDS](https://www.usds.gov) and [GSA](https://www.gsa.gov/), as well as vendor teams [TrussWorks](https://truss.works), [Coforma](https://coforma.io), and [ATI](https://atisolutions.us/).

Direct File also incorporates the Fact Graph, a declarative, XML-based knowledge graph data structure that is designed to reason about incomplete information, such as a partially completed tax return. The Fact Graph is written in the Scala programming language; it runs on the JVM on the backend and is transpiled via [Scala.js](https://www.scala-js.org) to run on the client as well. Direct File's Fact Graph is not domain-specific, and it may be useful to revenue agencies and as a reference for business rules engine implementations.

For a more details on the program and its history see https://www.irs.gov/pub/irs-pdf/p5969.pdf and https://www.irs.gov/filing/irs-direct-file-for-free
