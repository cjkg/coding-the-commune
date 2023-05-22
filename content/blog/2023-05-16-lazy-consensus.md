---
title:  "Lazy Consensus and the Problem of 'Endless Meetings'"
date:   2023-05-16
tags:
	- consensus
	- lazy consensus
	- endless meetings
---

In the standard case, collective decisions are made by a group of people in a room together. This arrangement requires planning on the part of the participants. Rooms need to be booked - at an inn, a library, a community center, or someone's house. Schedules have to be accommodated. Refreshments have to be prepared.

As time has gone on, the need for spatial and temporal proximity between participants has lessened. The COVID-19 pandemic has forced many of us to participate in collective decision-making from afar, via tools like Zoom, Teams, and Meet. Other communication tools like e-mail, Slack, and Discord allow us to conduct decision-making processes asynchronously, through voice and text messages. Discussions can be continued over several days without the need for late-night discussions or repeated bookings and reschedulings.

Obviously, not all collective decision-making can be done this way. Some collective decision-making needs all participants together, as the decisions may need to be made rapidly and require everyone see the current situation unfold. Some people do not have access to the aforementioned tools for remote decision-making. Some discussions are too sensitive to be recorded even on encrypted services like Signal.

Luckily, generally speaking, software development doesn't face these hurdles. We *can* conduct collective decision-making at a distance and asynchronously. And this simplifies all kinds of decision-making procedures for software development, but especially decisions by consensus. When conducting collective decision-making by consensus, a decision is made only if every participant in the project freely consents to the decision. So, no decision can be made unless no one in the project has any objections to the decision. 

But there's an obvious case that makes this arrangement difficult: emergency changes. When there's a critical bug in the code, we cannot wait for everyone to have a chance to voice any concerns. Someone needs to push the change as soon as possible. How can a project that makes decisions by consensus account for this?

### Lazy Consensus

The answer is *lazy consensus*, a method I briefly discussed in my introduction to [software by consensus](/blog/2023-05-06-software-by-consensus/). Lazy consensus allows a smaller group of participants to change the code without holding a discussion about the change first. Lazy consensus is possible with software development, because distributed version control tools, like Git or Mercurial, give us a "Time Machine" to roll back the changes if anyone disagrees after the fact. This is a fairly unique luxury that is built into software projects: most other decisions, once made, cannot be undone.

Besides allowing for quick emergency changes, lazy consensus mitigates a classic criticism of consensus decision-making - namely, that it leads to "endless meetings." If we need to have consensus on every decision, then we will need to hold a meeting for every decision. Compare this with organizations that elect officers, who can quickly make decisions in lieu of the participants of the organization's project(s). Although highly relevant to software projects, the debate between consensus and majority rule is most commonly found in the realm of leftist politics. Typically, majoritarian socialist organizations, such as the [Bread and Roses caucus](https://breadandrosesdsa.org/where-we-stand/#democracy-not-horizontalism) of the Democratic Socialists of America, make this objection against libertarian-socialist and left-anarchist competitor organizations, which are typically consensus-based.

But lazy consensus greatly reduces the number of meetings needed, as trivial changes can go ahead without discussion beforehand. For example, no discussion needs to be held for the correction of a minor typo, as it is likely no one will object. On the other hand, if a change is not trivial, one can hardly complain about the need for a meeting, as it merits discussion. Between this, and modern communication tools, the number of meetings is greatly reduced.

### The Problem of Endless Meetings

However, this isn't the whole of the "endless meetings" objection, as one could accuse decision-making by consensus of being "endless" in *duration*. That is, they claim that reaching consensus is sometimes impossible, or takes too long to reach in many cases. One can argue that lazy consensus doesn't avoid this problem, as many discussions over significant, non-trivial issues will be interminable, or simply end in no change at all. Much more efficient, they say, is majoritarianism, which is the paradigm of decision-making that makes decisions by majority vote. When discussion begins to repeat itself, or becomes deadlocked, you put it to a vote and move on. 

The majoritarian critique of consensus thus makes two claims: one is that majoritarianism is generally more efficient than consensus; the second is that consensus is *prohibitively* inefficient. 

The first claim is certainly true: generally speaking, any time consensus is reached on a decision after protracted debate, a majority decision would have been reached just as quickly, if not faster, due to an earlier majority vote. But a mere difference in efficiency is hardly a reason to reject decisions by consensus in favor of majoritarianism. That would be to say that consensus was without value, something the majoritarian can hardly claim, as a consensus decision is surely better than a fractious, divided one for the long-term health of a project. Consensus is the goal of all collective decision-making - even majoritarian organizations only resort to a vote when there is disagreement (Blunden 2016, 5). We will discuss this more in a later post.

Rather, we have to defeat the stronger, second claim, that consensus decision-making is *prohibitively* inefficient, which would cast doubt on lazy consensus as a viable collective decision-making procedure. 

But the inefficiency of consensus decision-making is an empirical claim about the world. Majoritarian political organizations, like Bread and Roses, often *state* that consensus decision-making leads to failure and breakdown of projects. However, they typically simply provide anecdotes of consensus's worst-case scenarios of long, bitter debates, without providing any evidence that these scenarios are representative. 

And we too could provide anecdotal data if we wished: plenty of successful software projects operate by lazy consensus. But setting dueling anecdotes aside, research suggests consensus is hardly prohibitively inefficient: in a rare study on consensus decision-making's efficiency, it was found that the average debate time, *in person*, took 2 hours for the organizations surveyed (Leach 2016). Some groups are faster than others, of course, and Leach's research suggests that the time to reach consensus is improved by: familiarity with decision-making by consensus; belief in the importance of reaching consensus; meeting more frequently; and personal investment in the project (Leach 2016, 53). Interestingly, Leach's research found no correlation between number of participants and efficiency, nor did the age of the organization seem to play a role (Leach 2016, 53).

### Further Questions

Exactly what lessons we can draw from Leach's research for software development projects that are done at a distance and asynchronously is hard to say. What we can conclude, though, from Leach and anecdotal evidence is that lazy consensus does not *inherently* lead to "endless meetings" to resolve issues. Obviously, more difficult and serious questions may take a very long time to resolve, but that is precisely because they are difficult and serious decisions. Is this a problem? That depends on how you answer a number of questions:
- Ethical and value judgments
	- Is the process of debate and reaching a consensus inherently valuable?
	- Does overruling the disagreement of minority voices violate their rights of autonomy?
- Practical questions
	- Does the value of efficiency outweigh the risks of ignoring some participants' reservations?
	- Does the value of efficiency outweigh the risks of long-term incoherence in a project, due to multiple different visions of the project?

These are questions I will address in the next post.

### Acknowledgements

Thanks to Preston J. Werner for valuable discussion.

### Bibliography

Blunden, Andy. 2016. *The Origins of Collective Decision-Making.* Brill, 2016 (also available at [Haymarket Books](https://www.haymarketbooks.org/books/998-the-origins-of-collective-decision-making))

Leach, Darcy K. 2016. "When Freedom Is Not an Endless Meeting: A New Look at Efficiency in Consensus-Based Decision Making." The Sociological Quarterly 57, no. 1 (2016): 36-70.