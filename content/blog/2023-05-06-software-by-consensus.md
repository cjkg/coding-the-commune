---
title:  "Software by Consensus"
date:   2023-05-06
tags:
	- consensus
---
The goal of this post is to carve out some ideal types of software development projects, where decisions are made by consensus (or rough consensus). This exercise is, in part, to lay the groudwork for other posts that imagine what software development would look like in a more equitable future society, as well as to identify some projects that prefigure such an arrangement.

We will get into what making decisions by consensus means, and compare it to other forms of collective decision making below. But first, we must start with more primitive concepts.

## Projects

Human beings work on projects. The relevant concept of a project is difficult to define, but it can be characterized. First, projects are (for this discussion) a group activity. They involve participants coming together to do *something*. Second,  participants in a project come together in *good faith* to pursue their *shared interests* (although they can certainly disagree on much else). A group pursuit of shared interests forms *a collective will* to do something - in our case, create software.

This leads to an important corollary: not all groups activities are projects. For example, when a company hires someone to write some code, this does not constitute a project, because the employer and the employee do not share the same interests, and therefore do not form a collective will. The employee is at the *command* of the employer, and pursues the employer's interest in exchange for wages. In this sense, our use of the word project is idiosyncratic, but I hope not too much so.

## Participants

In the kind of software project we are interested in, a participant is anyone who has a voice in the project. In software, participants in the project are not just the developers. Participants also include users, testers, and reviewers (where a reviewer ultimately approves the change). The role of users is particularly complex and will be set aside for another post.

Everyone in the community behind a project *can* play some or all the roles simultaneously. In the limit case, everyone in the community works on the project as a developer, a tester, and a reviewer -- and these same people are the only users of the software. This kind of equilibrium is uncommon simply because most of us want our software to be used widely and be put to good use. This would be impossible if we limited use of software to those who were actively developing, testing, and reviewing the software. (This kind of project need not be exclusionary: it might just so happen that no one needs the software outside the small group of people directly building it.) 

(As an aside, we're assuming that all participants have access to the source code at all stages of development. Otherwise how would participants make collective decisions about changes to the code? As a result, we are not so much interested in the Cathedral versus the Bazaar distinction Eric S. Raymond draws [apologies for having to bring him up], at least for now.)

## Decisions

So now we come to collective-decision making: when a change is proposed, how do participants decide whether to implement it? What I've hinted at is that such decisions could be made by consensus. But that is not the only paradigm of collective decision making. Following the work of Andy Blunden in his [The Origins of Collective Decision-Making](https://www.haymarketbooks.org/books/998-the-origins-of-collective-decision-making) (pp. 4-5), we will consider three paradigms (summarizing Blunden):
  - **Majoritarianism**: When a project's participants can't come to a consensus on what to do, it is put to the vote. Everyone's vote is equal, and when the votes are tallied, the majority carries the day. Those in the minority do not have the right to block the majority's will once the votes are cast, and their participation in the project binds them to this commitment.
  - **Consensus**: A decision is made only if every participant in the project freely consents to the decision. In projects that require consensus to make decisions, minority views have a great deal of weight, and the stability of the status quo is therefore favored over rapid innovation. Participants who disagree with the decision, but do not want to block progress, may "stand aside" (although participants frequently standing aside is a sign that the consensus decision-making of a project has deteriorated).
  - **Counsel**: When decisions are made by counsel, one particular person (a king, Linus Torvalds, etc.) takes the *counsel* of the other participants, but ultimately is the person who alone makes the decision based on that advice. The person who accepts counsel may delegate or rubber-stamp decisions, but ultimately they are the decision maker.

## The How and Why Consensus
