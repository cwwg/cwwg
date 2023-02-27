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

This document.

# Motivation

We need to define our RFC process so that we know how the other RFCs will be structured.

# Detailed design

RFCs are listed in the `rfcs/` directory and follow the same structure as this RFC. If they are on branch `main`, then they are considered to be **active**. If they are still in a PR, then they are not active yet. Discussion surrounding the RFC happens in **GitHub Discussions**.

Here's a detailed example of the creation of an RFC that defines a new documentation system:

1. We create a new branch: `rfc-documentation-system`. Either from a fork or on the monorepo itself.
2. We run `cd rfcs && cp 0000-template.md 0000-documentation-system.md`. Note that the number of a new RFC is always 0000.
3. We open `0000-documentation-system.md` and fill out the template.
4. We push our branch and open an  **Introduction PR**.
5. We create a new **Reference Discussion** on the [RFCs Discussions page](https://github.com/cwwg/cwwg/discussions/categories/rfcs) with the following title: "RFC: Documentation System".
6. We edit `0000-documentation-system.md` to include references to the **Introduction PR** and **Reference Discussion** and push this change. 
7. We discuss the PR in the **Reference Discussion**.
8. If you want to make a suggestion to an RFC that is in a PR, you can add a PR comment/suggestion to it.
9. Once two members from @cwwg/core approve the **Introduction PR**, the RFC gets merged and becomes active. When this happens, the RFC's number is changed from `0000` to the highest currently active RFC's number + 1.

# Drawbacks

- Having a formal RFC system may seem too bureaucratic to some.
- RFCs may become overly verbose. We should keep them as short and focused as possible, while still keeping them unambiguous.

# Alternatives

None so far. We mostly based this on [Vue.js' RFC process](https://github.com/vuejs/rfcs/blob/master/0000-template.md). We propose to try this out, and adjust the process if needed.

# Adoption strategy

Since there are no other RFCs yet, this RFC will not introduce any breaking changes. Adoption should be straightforward, anyone reading this RFC should immediately understand how the process will work.