---
title:  "Lazy Consensus"
date:   2023-05-16
tags:
	- consensus
---

In the standard case, collective decisions are made by a group of people in a room together. This arrangement requires planning on the part of participants. Rooms need to be booked -- at an inn, a library, a community center, or someone's house. Schedules have to be accommodated. Refreshments have to be prepared.

As time has gone on, these requirements have lessened the need for spatial and temporal proximity between participants. The COVID-19 pandemic has forced many of us to participate in collective decision-making from afar, via tools like Zoom, Teams, and Meet. Other communication tools like e-mail, Slack, and Discord allow us to conduct decision-making processes asynchronously, through voice and text messages. Discussions can be continued over several days without the need for late-night discussions or repeated bookings and reschedulings.

Obviously, not all collective decision-making can be done this way. Some collective decision-making needs all participants together, as the decisions may need to be made rapidly and require everyone see the current situation unfold. Some people do not have access to the aforementioned tools for remote decision-making. Some discussions are too sensitive to be recorded even on encrypted services like Signal.

Luckily, generally speaking, software development doesn't face these hurdles. We *can* conduct collective decision-making at a distance and asynchronously. But there's a particular case that makes this arrangement difficult: emergency changes. When there's a critical bug in the code, we cannot wait for everyone to have a chance to voice any concerns. Someone needs to push the change as soon as possible. How can consensus account for this?

The answer is *lazy consensus*, a method I discussed in my introduction to (software by consensus)[/blog/2023-05-06-software-by-consensus/]. Lazy consensus allows a smaller group of participants to change the code without holding a discussion about the change first. Lazy consensus is possible with software development, because distributed version control tools, like Git or Mercurial, give us a "Time Machine" to roll back the changes if anyone disagrees. This is a fairly unique luxury that is built into software projects: most other decisions, once made, cannot be undone.

Besides allowing for quick emergency changes, lazy consensus mitigates a classic criticism of consensus: that decision-making by consensus leads to "endless meanings." For lazy consensus greatly reduces the number of meetings needed, as trivial changes can go ahead without discussion beforehand. For example, no discussion needs to be held for the correction of a minor typo, as it is likely no one will object. On the other hand, if a change is not trivial, one can hardly complain about the need for a meeting, as it merits discussion.

However, this isn't the whole of the "endless meetings" objection, as one could accuse decision-making by consensus of being "endless" in duration. That is, they claim, reaching consensus is sometimes impossible, or takes too long to reach in many cases. One can argue that lazy consensus doesn't avoid this problem, as many meetings over significant, non-trivial issues will be interminable, or end in no change. Much more efficient, they say, is majoritarianism, which is the paradigm of decision-making that makes decisions by majority vote. When discussion begins to repeat itself, or becomes deadlocked, you put it to a vote and move on. (Although highly relevant to software projects, the debate between consensus and majority rule is most commonly in the realm of leftist politics, where majoritarian socialist organizations, such as the (Bread and Roses caucus)[https://breadandrosesdsa.org/where-we-stand/#democracy-not-horizontalism] of the Democratic Socialists of America, criticize libertarian-socialist and left-anarchist competitor organizations, which are typically consensus-based.)

The majoritarian critique of consensus thus makes two claims: one is that majoritarianism is generally more efficient than consensus; the second is that consensus is *prohibitively* inefficient. 

The first claim is certainly true: generally speaking, any time consensus is reached on a decision after protracted debate, a majority decision would have been reached just as quickly, if not faster, due to an earlier majority vote. But a mere difference in efficiency is hardly a reason to reject decisions by consensus in favor of majoritarianism. That would be to say that consensus was without value, something the majoritarian can hardly claim, as a consensus decision is surely better than a fractious, divided one. Consensus is the goal of all collective decision-making -- even majoritarian organizations only resort to a vote when there is disagreement (Blunden XXXX).

Rather, we have to defeat the stronger, second claim, that consensus decision-making is *prohibitively* inefficient, which would cast doubt on consensus as a viable collective decision-making procedure. 

But the inefficiency of consensus decision-making is an empirical claim about the world. Majoritarian political organizations, like Bread and Roses, often *state* that consensus decision-making leads to failure and breakdown of projects. However, they typically simply provide anecdotes of consensus's worst-case scenarios of long, bitter disagreements, without providing any evidence that these scenarios are representative. And we too can also provide anecdotal data: plenty of successful software projects operate by consensus, and do not fail in their goals. For example, is there any technological project with more reliable results than the consensus-based Internet Engineering Task Force, which crafts the Internet Protocol Suite (TCP/IP)? 

But setting dueling anecdotal aside, empirical research does not bear out the claim that consensus is hopelessly inefficient.

https://producingoss.com/en/consensus-democracy.html
https://en.wikipedia.org/wiki/Internet_protocol_suite
https://medlabboulder.gitlab.io/democraticmediums/mediums/lazy_consensus/
https://humanwhocodes.com/blog/2015/04/14/consensus-driven-development/