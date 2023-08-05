---
layout: post
title: Pragmatic path towards self-driving
date: 2023-08-04 23:39 -0700
description: Tesla and comma.ai have potential advantages in solving self-driving at scale due to their access to large volumes of end-to-end human driving data and pragmatic approaches of focusing on minimal components.
image:
category: business
tags: strategy
comments: true
---

Among dozens of companies trying to solve general self-driving at scale, two companies acknowledge the complexity of the physical world and demonstrate a pragmatic approach: Tesla and comma.ai.

Driving takes between 20-120 hours to learn and 3-6 months to practice across different countries; comparing it to other tasks such as learning a foreign language, which takes 600-1,800 hours, makes it relatively easy. Humans use vision from two eyes with the help of mirrors, and operate the wheel, brake and pedal. People seem to generalize well and know how to handle traffic cones if needed [^1].

For modern-day self-driving systems, multiple sensors like cameras and LiDARs give self-driving cars a much broader and more detailed view of the environment than human senses. This hardware advantage should enable better driving capability over human eyes and mirrors. The reason they still cannot handle unseen cases is likely an issue with the model itself or the training objective of the models. Most systems break the entire system into components such as perception, comprehension, and control systems, each trained with sub-objectives. Composing such a system requires careful design of the API between each component, which there is no guarantee humans would do better than machines.

The progress made by LLMs shows a promising combination of the right model with a large volume of data. With a simple transformer-based model, it learns knowledge and generalizes concepts equivalent to a top undergraduate student. Its success validates probable guidelines for AI systems:
- Complexity could emerge from simple rules[^2]
- End-to-end learning with the right architecture is capable of generalization
- A model that learns from human behaviors would behave like a human

Let's imagine developing a new self-driving car system using the guidelines revealed by LLMs:
- The system will be trained end-to-end from perception to control actions.
- The training would need large volumes of human behavior data.

The progress of model development in industry is a process similar to the evolutionary process[^3], where "search is at its most awesome when it has no unified objective". Therefore, knowledge sharing is a dominating culture both in academia and industry for AI research; and model architecture hasn't been used as a commercial barrier of entry.

Then, the barrier to solving the modeling problem of self-driving would be human driving behavior data. Among all self-driving companies, who has the most human driving data? Tesla. As of Q3 2022, Tesla has delivered over 3.3 million vehicles total and is delivering ~350,000 every quarter. Traditional car manufacturers don't have the infrastructure to capture end-to-end data, and technology companies like Cruise and Waymo don't have as much human driver data as Tesla [^4].

Besides intelligence, another complexity for planet-scale self-driving deployment is hardware complexity. There are over 100 well-known car manufacturers worldwide, each with different control systems that also evolve. Despite solving the abstract sensing-acting problem, without integrating with hardware, deployment would not be scalable. Tesla addresses this by controlling complexity itself, and its consumer success has increased its market share.

Companies in possession of large volumes of end-to-end human behavior data and hardware knowledge have a chance to win the self-driving race. Another company with a chance is comma.ai[^5]. It focuses its product on the two minimal components of end-to-end self-driving and relies on crowd-sourcing software to deploy to multiple cars. It owns the end-to-end data pipeline and addresses the remaining market share of vehicle hardware besides Tesla. Its strategy would allow it to grow faster than Tesla as it can deploy onto vehicles already on the road.

Additionaly, The frameworks of Tesla and comma.ai position them advantageously in the race towards self-driving capabilities. Their potential for economies of scale comes from the large volume of vehicles they produce or deploy, and the continuous data collection these vehicles enable. Every new customer expands their data collection network, contributing to the enhancement of their autonomous systems.

## Conclusion
End-to-end human behavior data collection and hardware integration advantages put Tesla and comma.ai in a promising position to solve self-driving; with economical scaling, both have shown a pragmatic approach for a future with self-driving deployed as planet scale.

---

[^1]: [The Self-Driving Cars stopped by traffic cones put by activists.](https://slate.com/business/2023/07/autonomous-vehicles-traffic-cones-san-francisco-cruise-waymo-cpuc.html)
[^2]: [Stephen Wolfram explains his philosophy on complexity](https://www.youtube.com/watch?v=UjL_N0SLLSc)
[^3]: [Book summary of Why Greatness Cannot Be Planned](https://blas.com/why-greatness-cannot-be-planned/)
[^4]: Waymo has 20+ billions simulated road miles and 20+ millions real-world miles.[ref](https://waymo.com/waymo-driver/#:~:text=The%20Waymo%20Driver%20takes%20the,other%20road%20users%20might%20do.)

[^5]: https://github.com/commaai/openpilot