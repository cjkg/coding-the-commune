---
title:  "Software by Consensus"
date:   2023-05-15
tags:
	- consensus
---
The goal of this post is to carve out some ideal types of software development projects, where decisions are made by consensus (or rough consensus). This exercise is, in part, to lay the groundwork for other posts that imagine what software development would look like in a more equitable future society, as well as to identify some currently existing projects that prefigure such an arrangement.

We will get into what making decisions by consensus means, and compare it to other forms of collective decision-making below. But first, we must start with more primitive concepts.

## Projects

Human beings work on projects. The relevant concept of a project is difficult to define, but it can be characterized. First, projects are (for this discussion) a group activity. They involve participants coming together to do *something*. Second,  participants in a project come together in *good faith* to pursue their *shared interests* (although they can certainly disagree on much else). A group pursuit of shared interests forms *a collective will* to do something - in our case, create software.

This leads to an important corollary: not all groups activities are projects. For example, when a company hires someone to write some code, this does not constitute a project, because the employer and the employee do not share the same interests, and therefore do not form a collective will. The employee is at the *command* of the employer, and pursues the employer's interest in exchange for wages. In this sense, our use of the word project is idiosyncratic, but I hope not too much so.

## Participants

In the kind of software project we are interested in, a participant is anyone who has a voice in the project. In software, participants in the project are not just the developers. Participants also include users, testers, and reviewers (where a reviewer ultimately approves the change). The role of users is particularly complex and will be set aside for another post.

Everyone in the community behind a project *can* play some or all the roles simultaneously. In the limit case, everyone in the community works on the project as a developer, a tester, and a reviewer -- and these same people are the only users of the software. This kind of equilibrium is uncommon simply because most of us want our software to be used widely and be put to good use. This would be impossible if we limited use of software to those who were actively developing, testing, and reviewing the software. (This kind of project need not be exclusionary: it might just so happen that no one needs the software outside the small group of people directly building it.) 

(As an aside, we're assuming that all participants have access to the source code at all stages of development. Otherwise how would participants make collective decisions about changes to the code? As a result, we are not so much interested in the Cathedral versus the Bazaar distinction Eric S. Raymond draws [apologies for having to bring him up], at least for now.)

## Decisions

So now we come to collective decision-making: when a change is proposed, how do participants decide whether to implement it? What I've hinted at is that such decisions could be made by consensus. But that is not the only paradigm of collective decision-making. Following the work of Andy Blunden in his [The Origins of Collective Decision-Making](https://www.haymarketbooks.org/books/998-the-origins-of-collective-decision-making) (pp. 4-5), we will consider three paradigms (summarizing Blunden):
  - **Majoritarianism**: When a project's participants can't come to a consensus on what to do, it is put to the vote. Everyone's vote is equal, and when the votes are tallied, the majority carries the day. Those in the minority do not have the right to block the majority's will once the votes are cast, and their participation in the project binds them to this commitment.
  - **Consensus**: A decision is made only if every participant in the project freely consents to the decision. In projects that require consensus to make decisions, minority views have a great deal of weight, and the stability of the status quo is therefore favored over rapid innovation. Participants who disagree with the decision, but do not want to block progress, may "stand aside" (although participants frequently standing aside is a sign that the consensus decision-making of a project has deteriorated).
  - **Counsel**: When decisions are made by counsel, one particular person (a king, a benevolent-dictator-for-life, etc.) takes the *counsel* of the other participants, but ultimately it is that one person alone who makes the decision. Even though it is undemocratic, it is a case of collective decision-making. Every participant in the project has a voice, even if their voice is not equal.

## The Basics of Consensus

The consensus model of decision-making requires that everyone consent to the proposed action(s). In that sense, any one participant can veto any proposal. This is radically different from majoritarianism where one "no" vote can only negate one "yes" vote, and vice versa. Under the consensus model, a "no" vote is all powerful, as no amount of "yes" votes can overcome it. Minority views are thereby "treasured" by the consensus model, while they are merely tolerated in the majoritarian model (Blunden, 5). Even so, wrongheaded or lasting disagreement is typically not tolerated in consensus, and can lead to expulsion from the project or informal sanctions. But for all this talk of voting and vetoes, it's really only a figure of speech: there is no voting in the consensus model, there is only consensus or dissent. Those are the only two states that matter. As a result, there's no sense in counting every "vote" other than to help guide discussion. Further, unlike in other contexts, silence counts as consent, requiring no "vote" to be cast in order to agree.

## Consensus and Software

Consensus may seem completely implausible as a method for making decisions in a software development project, especially if, like me, you come from a corporate programming background. But there are features of software development that make it particularly suited to decision-making by consensus. 

The first is that version control tools, like Git, give us a "time machine", which allows for ["lazy consensus."](https://community.apache.org/committers/lazyConsensus.html) That is, a participant of a project can make a change to the software if they believe it would have reached consensus (*e.g.*, a critical bug-fix) because it can always be rolled back if anyone objects. This eliminates one of the most frustrating aspects of consensus decision-making: the need to discuss every decision, especially on very short notice. Lazy consensus has been implemented with great success at the [Apache Foundation](https://community.apache.org/).

The second feature that makes consensus suited for software development is that software development decisions lend themselves to asynchronous communication. Collaborating on software is much different than collaborating on laying railroad tracks, cutting down trees, or conducting spacewalks. There is generally no need for eye contact, instantaneous communication, or spatial proximity. As a result, discussions are easily conducted using tools like mailing lists, slack, GitHub issue threads, etc. This makes meetings easier to hold, as there is no requirement for scheduling to make sure everyone can make it.

The final feature of software development that makes it suited for consensus decision-making is distributed version control tools, like Git and Mercurial. Such tools allow for decentralization of projects, as in a distributed version control system, there is no centralized codebase. Every participant of the project can have the full codebase and its history of changes locally on their machine, and can propose changes for everyone's consideration. Without the distributed nature of these systems, some subset of the project's participants would be gatekeepers to the "pristine" codebase, and could lock dissident voices out. Further, if the project devolves, the codebase is easily forked into another project.

## Conclusion

In the next few posts, I plan on discussing these features of software development in greater depth. The next post will discuss lazy consensus and the Apache project. After that I will turn to the history of Git and how its structure enables different kinds of collective decision-making, focusing mostly on consensus.