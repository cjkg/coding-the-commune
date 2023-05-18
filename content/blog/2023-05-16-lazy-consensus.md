---
title:  "Lazy Consensus"
date:   2023-05-16
tags:
	- consensus
---
In the standard case, collective decisions are made by a group of people in a room together. This arrangement requires planning on the part of participants. Rooms need to be booked -- at an inn, a library, a community center, or someone's house. Schedules have to be accommodated. Refreshments have to be prepared.

As time has gone on, these requirements have lessened the need for spatial and temporal proximity between participants. The COVID-19 pandemic has forced many of us to participate in collective decision-making from afar, via tools like Zoom, Teams, and Meet. Other communication tools like e-mail, Slack, and Discord allow us to conduct decision-making processes asynchronously, through voice and text messages. Discussions can be continued over several days without the need for late-night discussions or repeated bookings and reschedulings.

Obviously, not all collective decision-making can be done this way. Some collective decision-making needs all participants together, as the decisions may need to be made rapidly and require everyone see the current situation unfold. Some people do not have access to the aforementioned tools for remote decision-making. Some discussions are too sensitive to be recorded even on encrypted services like Signal.
is
Luckily, generally speaking, software development doesn't face these hurdles. We *can* conduct collective decision-making at a distance and asynchronously. But there's a particular case that makes this arrangement difficult: emergency changes. When there's a critical bug in the code, we cannot wait for everyone to have a chance to voice any concerns. Someone needs to push the change as soon as possible. How can consensus account for this?

The answer is *lazy consensus*, a method I discussed in my introduction to [software by consensus---
title:  "Lazy Consensus"
date:   2023-05-16
tags:
	- consensus
---
In the standard case, collective decisions are made by a group of people in a room together. This arrangement requires planning on the part of participants. Rooms need to be booked -- at an inn, a library, a community center, or someone's house. Schedules have to be accommodated. Refreshments have to be prepared.

As time has gone on, these requirements have lessened the need for spatial and temporal proximity between participants. The COVID-19 pandemic has forced many of us to participate in collective decision-making from afar, via tools like Zoom, Teams, and Meet. Other communication tools like e-mail, Slack, and Discord allow us to conduct decision-making processes asynchronously, through voice and text messages. Discussions can be continued over several days without the need for late-night discussions or repeated bookings and reschedulings.

Obviously, not all collective decision-making can be done this way. Some collective decision-making needs all participants together, as the decisions may need to be made rapidly and require everyone see the current situation unfold. Some people do not have access to the aforementioned tools for remote decision-making. Some discussions are too sensitive to be recorded even on encrypted services like Signal.
is
Luckily, generally speaking, software development doesn't face these hurdles. We *can* conduct collective decision-making at a distance and asynchronously. But there's a particular case that makes this arrangement difficult: emergency changes. When there's a critical bug in the code, we cannot wait for everyone to have a chance to voice any concerns. Someone needs to push the change as soon as possible. How can consensus account for this?

The answer is *lazy consensus*, a method I discussed in my introduction to (software by consensus)[/blog/2023-05-06-software-by-consensus/]. Lazy consensus allows a smaller group of participants to change the code without holding a discussion about the change first. Lazy consensus is possible with software development, because distributed version control tools, like Git or Mercurial, give us a "Time Machine" to roll back the changes if anyone disagrees. This is a fairly unique luxury that is built into software projects. Most decisions, once made, cannot be undone.
