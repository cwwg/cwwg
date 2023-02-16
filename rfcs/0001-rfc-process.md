- Start Date: 2023-02-16
- Reference Discussion: cwwg/cwwg#6
- Introduction PR: cwwg/cwwg#8
- Implementation PR: cwwg/cwwg#8

# Summary

The RFC process has the following structure:

- The top level `rfcs/` directory on branch `main` contains all active RFCs.
- Each RFC has the following linked at the start:
  - **Reference Discussion**: Threaded discussion for discussing the RFC.
  - (**Reference Issues**): If applicable, a list of issues that inspired this RFC.
  - **Introduction PR**: The PR introducing the RFC itself
  - (**Implementation PR**): If applicable, a PR demonstrating an implementation of the proposed changes.
- Once an RFC's **Introduction PR** is approved by @cwwg/core, it gets merged into `main` and becomes an active RFC.

# Basic example

We want to create an RFC which defines a new documentation system.

1. We create a new branch: `rfc-documentation-system`. Either from a fork or on the monorepo itself.
2. We run `cd rfcs && cp 0000-template.md 0000-documentation-system.md`. Note that the number of a new RFC is always 0000.
3. We open `0000-documentation-system.md` and fill out the template.
4. We push our branch and open an  **Introduction PR**.
5. We create a new **Reference Discussion** on the [RFCs Discussions page](https://github.com/cwwg/cwwg/discussions/categories/rfcs) with the following title: "RFC: Documentation System".
6. We edit `0000-documentation-system.md` to include references to the **Introduction PR** and **Reference Discussion** and push this change. 
7. We discuss the PR in the **Reference Discussion**.
8. Once someone from @cwwg/core approves the **Introduction PR**, the RFC gets merged and becomes active.

# Motivation

Why are we doing this? What use cases does it support? What is the expected
outcome?

Please focus on explaining the motivation so that if this RFC is not accepted,
the motivation could be used to develop alternative solutions. In other words,
enumerate the constraints you are trying to solve without coupling them too
closely to the solution you have in mind.

# Detailed design

This is the bulk of the RFC. Explain the design in enough detail for somebody
familiar with the CWWG to understand, and for somebody familiar with the
implementation to implement. This should get into specifics and corner-cases,
and include examples of how the feature is used. Any new terminology should be
defined here.

# Drawbacks

Why should we *not* do this? Please consider:

- implementation cost, both in term of code size and complexity
- whether the proposed feature can be implemented in user space
- the impact on teaching people about the CWWG
- integration of this feature with other existing and planned features

There are tradeoffs to choosing any path. Attempt to identify them here.

# Alternatives

What other designs have been considered? What is the impact of not doing this?

# Adoption strategy

Will this RFC introduce breaking changes of any kind? If so, how will we facilitate migrations?

# Unresolved questions

Optional, but suggested for first drafts. What parts of the design are still
TBD?