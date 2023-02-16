- Start Date: 2023-02-16
- Reference Discussion: cwwg/cwwg#9
- Implementation PR: cwwg/cwwg#8

# Summary

Core members of CWWG need a well-defined, efficient, and asynchronous way to
communicate with each other and with the community. This RFC defines ways
to achieve that.

# Motivation

Communicating well in a working group like this is essential since this group
consists of diverse teams and people from all around the world. Also, since
the core team members can be very busy with their day-to-day jobs, ways of
communication should be well defined and efficient as possible.

# Detailed design

A good structure for communication should be:
1. **Sustainable**: Core members should not be overwhelmed and should be able
to do their work consistently over a long period.
2. **Efficient**: Ways of communication should be efficient such that it shouldn't
take too much effort and also it shouldn't be done over and over again about the
same topic because of lack of structure. For example, Telegram can be a very fast
way to discuss a topic but it is easy to forget and hard for other people to follow.
3. **Transparent**: The community or any core members shouldn't get confused about where
a decision is coming from, why a feature is added or what are the plans for the future.
It should be the core team's mission to be transparent as possible. This will also
reduce the people's need for support and questions, hence the core team can focus more
on the actual work that they are doing.

By following these principles, the following elements can be applied:

1. Main channel for helping people should be GitHub issues. It is easy to find online,
participate, follow, and group.

2. For features, breaking changes, etc. RFC process should be followed.

3. For the issues that can turn into RFCs, members should motivate the community to
create an RFC and start a discussion (if the issuer is from the community). This will
motivate newcomers to be a part of the working group and take some heavy lifting.

4. Core members should be active in:
  - GitHub Issues,
  - RFC discussions/reviews,
  - PR reviews.
  
5. To group up and have a stable and solid plan, the core team should meet every 2 months.
These meetings should cover:
  - Overview of the current situation of the working group.
  - The things that have been done in the previous period.
  - Reviewing RFCs. Prioritizing the implementation.
  - Reviewing community feedback. This feedback can come from any channel.
  - Planning for the next period. Reviewing tasks and having a clear goal for the next meeting.
  
6. For chatting, quick discussions, and ideas, Telegram group can be used. Note that
requesting new features, and introducing big changes should not be done in the Telegram group.
Issues, discussions, and RFCs are already serving that purpose. Telegram should be
used for quick day-to-day matters, quick syncs, and internal discussions.

# Drawbacks

- The more the community gets involved in this group, having a meeting every 2 months might not be enough,
but it is always easy to change later.
- Community might not like having an interactive platform like discord but I think GitHub issues
are more sustainable and easy for other people to follow.

# Alternatives

- Other platforms like discord, slack, mattermost, etc. can also be used for grouping the discussions
and having separate concerns. But note that this can easily get out of control and things that are needed
to be discussed in GitHub issues/RFCs/discussions can be started to be discussed on these platforms.