---
permalink: /anecdotes/
title: Personal Anecdotes
author_profile: true
redirect_from:
  - /anecdote
---
My personal motivations behind each research project I'm currently working on.

## Fine-grained information retrieval for scientific literature 
I used to work in a web lab for preclinical stage medicinal chemistry synthesis. The research process was rather repetitive and tedious. Given a scaffold, I needed to couple it with different functional groups to find a promising drug candidate. The entire process of picking up a random functional group, looking up reaction conditions in relevant literature, running coupling reactions (usually I needed to run several trials experimenting with different reaction conditions to get a successful run), purifying and assessing under NMR took several weeks per cycle. I was lucky enough that I found a relatively competitive candidate in just 6 months. The unlucky PhD student from the lab next door had spent a whole year doing trial and errors but could not find any potent candidates. 

That was my first-hand experience of the long development timeline for novel drug discovery. Most of the decision makings (which functional groups to add, which catalyst should be used, etc.) are solely based on intuitions. To me, the repetitive trials were like spinning a wheelchair and trying to stop at a specific point, since there are no quantifiable objectives to really guide in this process. 

Different from retrosynthesis, reaction condition recommendation / optimization received much less attention and is overlooked in the AI for science field. But it remains critical in synthetic chemistry, as it directly impacts the yield rate of desired product. Numerous search time in synthetical chemistry for novel compounds is devoted to exploring effective reaction conditions. 

Is there a way to shift this paradigm from intuition-driven to more information-driven? In other words, can we utilize reaction conditions of similar reactions reported in published papers to constrain the search space of reaction conditions in a more informed manner rather than solely based on chemists’ intuitions? There are previous works focusing on utilizing RAG to better address reaction condition recommendation. Although they claim to show exceptional performance on automatic benchmarks, they are still a bit far from real-world applications. I have manually checked nearly 100 test cases, finding that only the ones that correctly retrieved corresponding gold text from the corpus predicted correct conditions. So this problem is effectively reduced into information retrieval. 

Current scientific search engines fail to retrieve the most relevant papers with relevant experiment conditions. Rather, I was heavily relying on “prompting” my PI to pinpoint relevant literatures for those specific compounds. Can we dive 

Can we delve into an even more fine-grain level (reaction level in synthetical chemistry) and potentially liberates chemists from weeks of trial and error for getting their reaction running?


## Making clinical documents readable to non-professionals
One of my family members was previously diagnosed with a terminal disease. The treatment plan for terminal conditions is really different from typical diseases – doctors will present a list of treatment plans and the patient will decide which one to proceed, since it is a trade-off between life expectancy and quality of life. 

Informed decision making is extremely important in this scenario. However, due to the overwhelming complexity of medical language as well as complicated clinical metrics, it is rather challenging for us, non-professionals, to fully understand what is going on. Although the doctor said “you are always welcome to call back for any questions you have, we are available 24/7”. However, we don’t even know what questions should be asked. We were given lengthy reports consisting of various clinical metrics. Due to inherent insurance billing issues, clinical documents often include a number of negative diagnoses in addition to positive ones, distracting the general public from navigating their real medical conditions. 

This inspired me to build a system to help the general public to be more informed about their medical conditions given their clinical documents and potentially help them to engage more actively in their care by asking more meaningful questions during doctor appointments




## Bridging communication gaps in interdisplinary science collaborations
Over the process of collaborating with researchers from the chemistry department, I find some of the joint group meetings to be rather exhaustive and ineffective, since two groups were not even on the same page most of the time. Science domain is extremely knowledge intensive. People from two completely disjoint disciplines are likely to have communication barriers due to the immense knowledge gap. According to my personal observations, people tend to overestimate their understanding in a domain they are not familiar with and over trust other people for their “appropriated” jargon at the same time. It is rather common to see an expert from the chemistry domain make a strong claim about some explicit machine learning tasks when they are actually describing something else. This will lead the conversation completely astray, making both groups confused since what the other group is describing completely mismatch with the technical terms they explicitly used. 

Because of this situation, we generally need multiple meetings spanning across a week to discuss something that is rather simple in one domain. This leads to my latest project investigating how to automatically enable smoother cross-domain communication. 






