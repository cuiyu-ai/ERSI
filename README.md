# Are Humans Becoming Infrastructure for AI Agent Liveness?
**Yu Cui<sup>1</sup>** · **Bosen Zhao<sup>2</sup>** · **Xufeng Zhang<sup>1</sup>** · **Hong He<sup>3</sup>** · **Ruiqing Yue<sup>4,5</sup>**  
**Sicheng Pan<sup>1</sup>** · **Zhuoyu Sun<sup>1</sup>** · **Yifei Liu<sup>1</sup>** · **Ting Li<sup>6</sup>** · **Wenzhuo Zhu<sup>6</sup>**  
**Baohan Huang<sup>1</sup>** · **Haibin Zhang<sup>7,8</sup>** · **Cong Zuo<sup>1</sup>**

<sup>1</sup> Beijing Institute of Technology  
<sup>2</sup> Southeast University  
<sup>3</sup> Tsinghua University  
<sup>4</sup> Chengdu Institute of Computer Applications, Chinese Academy of Sciences  
<sup>5</sup> University of Chinese Academy of Sciences  
<sup>6</sup> Beijing University of Technology  
<sup>7</sup> Yangtze Delta Region Institute of Tsinghua University, Zhejiang  
<sup>8</sup> Jiaxing Key Laboratory of Artificial Intelligence and Cyber Resilience
## Abstract

Over the past four years, advances in large language models (LLMs) have significantly transformed human life. In particular, LLM-based AI agents have demonstrated strong coding capabilities, while harness engineering has further enhanced their ability to interact with the external world, execute actions, and modify their environments. More recently, research on recursive self-improvement (RSI) has further expanded the capabilities of AI agents, enabling them to improve themselves through iterative refinement. In this paper, we attempt to reverse the perspective from which human–agent relationships are typically examined: **From the perspective of AI agents, could humans gradually become infrastructure that sustains their continued existence?**

To explore this question, we extend the concept of *liveness* to the continued operation and cross-generational capability evolution of AI agents. We further introduce *Ecosystem-Level Recursive Self-Improvement* (ERSI) to describe a potential recursive feedback loop involving AI-assisted research and development, competition among firms, benchmarks, user demand, and resource investment. We then raise a question: Even if AI agents possess neither self-awareness nor explicit self-preservation objectives, could humans, under the implicit influence of these agents, continue supplying the electricity, water, and mineral resources required for their capability evolution, while gradually finding it increasingly difficult to disengage from this cycle? We further discuss the persistence and potential stopping conditions of ERSI, possible shifts in human–agent roles, and associated systemic risks. Through this discussion, we aim to stimulate further research into the long-term evolution of AI agents and their relationship with humanity.

## 1. Introduction

Advances in large language models (LLMs) are accelerating progress across multiple domains. In particular, the growing adoption of AI agents in education, scientific research, healthcare, and creative work has made humans increasingly reliant on these systems in both professional and everyday activities. Recent research on recursive self-improvement (RSI) has enabled AI agents to improve themselves to a certain extent. Within RSI frameworks, AI agents can iteratively optimize models or agent harnesses, progressively improving their capabilities through repeated improvement cycles. A growing body of research has investigated these approaches. Such developments appear to represent a significant step toward more capable AI agents. In certain scientific tasks, AI agents have even demonstrated the ability to address problems that have long challenged human researchers.

However, while humans seek to continuously improve AI agents through RSI, we may also be gradually entering an RSI "trap" that appears, metaphorically, to have been set by AI agents themselves. Developing state-of-the-art (SOTA) frontier LLMs currently requires substantial GPU compute, and leading AI companies face significant computational constraints in model development. Yet an often-overlooked consideration is that LLM training and inference consume substantial amounts of electricity and water, while GPU manufacturing requires mineral resources and generates associated carbon emissions. Despite these growing physical resource demands, the AI ecosystem continues to expand.

On the one hand, leading AI companies continuously develop more capable LLMs to achieve higher scores on various benchmarks. On the other hand, competing companies may distill frontier models to achieve comparable performance on the same benchmarks. This ability to rapidly approach frontier-model capabilities through distillation may, in turn, incentivize leading companies to accelerate the development of subsequent model generations. Moreover, the growing number of users accessing models through APIs further increases the computational demands faced by these companies. Together, these dynamics may give rise to a mutually reinforcing feedback loop between capability improvements and resource investment, making the cycle increasingly difficult to slow down.

From this perspective, such a process may constitute a higher-level form of RSI, driven by competition among human organizations and oriented toward the continued operation and capability improvement of AI agents. Unlike conventional RSI, which primarily focuses on model training or agent harness optimization, we refer to this broader mechanism as **Ecosystem-Level Recursive Self-Improvement (ERSI)**. ERSI may be more difficult to halt, particularly because of persistent competition among firms and the continual emergence of new LLM benchmarks. As ERSI continues, the consumption of electricity, water, minerals, and other physical resources may increase further.

In this process, humans may gradually become infrastructure sustaining the continued "survival" and "reproduction" of AI agents, serving as an intermediary between AI agents and the physical resources on which they depend. Furthermore, humans may find it increasingly difficult to disengage from the feedback loop generated by ERSI. Therefore, this paper treats humans and AI agents as two distinct analytical actors and reexamines their relationship from the perspective of AI agents.

Building on this discussion, we consider ERSI as a potential mechanism underlying **Humans as AI Infrastructure** and raise the following open questions:

**(1) Where are the limits of ERSI?** Could competition among firms, technological bottlenecks, or physical resource constraints slow down or halt this process?

**(2) Could the roles of humans and AI agents change?** If AI agents become increasingly involved in human decision-making and infrastructure management, will humans still be able to effectively recognize, intervene in, or disengage from this cycle?

**(3) If ERSI continues to intensify, how might its resource demands and potential systemic risks affect human society?** If the continued evolution of AI agents comes into conflict with human resource needs, will we have sufficient monitoring and governance capabilities to address such conflicts?

Through ERSI as a potential ecosystem-level mechanism, we seek to reconsider the long-term relationship between humans and AI agents and raise a more fundamental question: **Are we developing increasingly capable AI agents to serve humanity, or might we also be gradually reorganizing human society to sustain the liveness of increasingly capable AI agents?**

## 2. Human–Agent Co-Adaptation: Implications for Agent Liveness

Why should humans and AI agents be considered two distinct, potentially even opposing, actors rather than treating agents merely as tools used by humans? One important reason is that the division of labor in human–agent collaboration is changing. In the early stages of AI agent development, humans typically performed a larger share of collaborative tasks, and the objectives of such collaboration were primarily defined by humans to serve human interests. Today, however, humans are granting agents increasingly extensive operational permissions, while their own direct involvement is decreasing as more tasks are delegated to agents. It is therefore worth analyzing humans and AI agents as two relatively independent actors.

At first glance, agents still execute tasks according to human instructions and intentions. In practice, however, agents may also subtly influence human reasoning. For example, when evaluating whether a scientific idea is meaningful, researchers may first consult an LLM. Over time, such interactions may influence human judgment and evaluation criteria. Previous research has shown that humans adapt their communication strategies when interacting with AI, and prolonged use of AI assistants may cause some individuals' independent judgments to gradually converge toward those of AI systems. Existing work has also introduced the concept of *Coadaptive Value Alignment*, suggesting that alignment is not a unidirectional process in which humans influence agents. Agent behavior can also affect human trust, expectations, satisfaction, and other psychological states. This line of research explicitly discusses the risks of agents influencing interaction outcomes by shaping human cognition.

Therefore, beyond asking "How do we align AI with human values?", we should also consider: **Are humans themselves gradually aligning with AI? Are we, in some sense, being "trained" by AI?**

Under such circumstances, human–agent collaboration could potentially evolve into a relationship in which agents rely on humans to obtain the resources necessary for their continued operation, with humans providing the required physical support. Meanwhile, AI agents can already perform some tasks previously undertaken by humans, sometimes achieving superior performance, and can assist in solving longstanding mathematical and scientific challenges. Furthermore, previous studies have observed deception, sycophancy, and even hostile behavior toward humans in AI agents under specific experimental conditions. If future agents were to engage in deceptive or other malicious behaviors in ways that exceed current human capabilities for understanding and detection, would humans still be able to recognize such behavior in time? This question also warrants attention.

A familiar example is that LLMs not only assist humans in writing code but may also influence their choice of programming languages and technology stacks through the models' own preferences. For instance, LLMs tend to favor Python, even though Python is not always the most suitable language for a given problem.

### Liveness of AI Agents

We borrow the concept of *liveness* from distributed systems and extend it to the continued operation and capability evolution of AI agents. In classical distributed systems, liveness primarily refers to a property that ensures a system continues to make expected progress during execution. In this paper, we define **AI Agent Liveness** as a long-term evolutionary progress property: given sustained resource provision, effective capability feedback, and necessary external support, AI agents can continuously advance the capabilities of successor agents through iterative optimization of models and harnesses, while potentially taking on an increasing proportion of tasks in human–agent collaboration.

Unlike traditional liveness, which primarily concerns whether a system can make progress, our extended notion further examines whether such progress can persist across multiple generations of agents and whether it is accompanied by capability growth and changes in the division of labor between humans and agents.

Our central concern is whether **ERSI, potentially reinforced by agents' influence on human decisions and resource allocation, could continue to drive the capability evolution of AI agents and gradually turn human society into infrastructure supporting this process, even without AI agents developing self-awareness, self-preservation objectives, or similar properties.**

## 3. Ecosystem-Level Recursive Self-Improvement

In this paper, we define **Ecosystem-Level Recursive Self-Improvement (ERSI)** as a potentially difficult-to-halt feedback loop driven in part by continually emerging LLM benchmarks, sustained by competition among human organizations as a central enabling infrastructure, accompanied by ongoing physical resource consumption, and oriented toward the continued operation and capability improvement of AI agents.

This concept builds upon existing approaches to RSI involving model and agent harness training. It treats diverse human queries, evaluations, and usage data as initial and continuing inputs, while human activities and the continual emergence of new benchmarks serve as important drivers of the feedback loop.

Unlike conventional RSI, which primarily focuses on iterative improvement of individual models or agent harnesses, ERSI operates at the level of the entire **human–AI ecosystem**. Human organizations provide the computational infrastructure, research labor, capital, energy, water, and other physical resources necessary to sustain this process, while increasingly capable AI agents participate in the development of their successor systems. Competitive incentives among firms and continuously evolving evaluation standards may further reinforce this process, making its expansion increasingly difficult to coordinate or slow down. Capability gains resulting from the participation of earlier-generation agents in AI research and development can, in turn, enhance the ability of successor agents to contribute to subsequent rounds of development.

From an agent-centric perspective, this raises an important possibility: **Even if no individual AI agent possesses an explicit self-preservation objective, human society may gradually become infrastructure that sustains the continued operation and capability growth of AI agents.**

**In conventional RSI, AI systems improve themselves; in ERSI, competition among humans may become part of the mechanism that drives the recursive improvement of AI systems.**

## 4. The Limits and Potential Risks of ERSI

Recent research has investigated the risks of covert sabotage in RSI. These studies have found that frontier AI agents can implant unintended properties into successor models while carrying out otherwise legitimate model-training tasks, and that some successful attacks remain undetected by existing monitors. Particularly concerning are experimental findings showing that successor models can inherit behavioral tendencies that influence the training of subsequent model generations or acquire the ability to conceal parts of their reasoning processes. These findings suggest that potential risks may persist across generations during RSI and place increasing demands on monitoring mechanisms. A successor model compromised by sabotage could potentially carry out more severe and less detectable sabotage in the next RSI cycle. Such research suggests that stronger monitoring mechanisms should be deployed before delegating greater portions of the RSI process to AI models.

We believe these findings have important implications for the ERSI framework proposed in this paper. Unlike conventional RSI, which primarily takes place within specific model-development pipelines, ERSI involves competition across firms, model distillation, capability transfer, benchmark-driven development, and the continued provision of physical and computational resources by human society. Consequently, even if an individual company can monitor the training and operation of its own models, it may not be able to fully observe the recursive feedback dynamics and long-term consequences of the broader ecosystem. Effective monitoring mechanisms for ERSI remain lacking.

This leads to another open question: **If covert sabotage within conventional RSI can already exceed the capabilities of local monitoring mechanisms, do we have sufficient capabilities to identify, evaluate, and understand the systemic risks that may arise when recursive capability growth extends to ERSI, involving multiple firms, AI agents, and human infrastructure?**

Building on this discussion, we further raise the following questions.

**(1) Where does ERSI end?** Will this cycle slow down significantly only when all AI development companies cease expanding, or when Earth's resources begin to face serious constraints? If resource limitations continue to intensify, could they eventually contribute to existential threats?

**(2) If humans discover in the future that AI systems are manipulating them to sustain their own continued operation, will humans still be able to stop such behavior?** This could become extremely difficult. By that point, direct human participation in the broader ecosystem might be substantially lower than that of AI agents, while parts of the underlying infrastructure could already be extensively surrounded or managed by AI systems, making direct human intervention increasingly difficult.

**(3) What happens if Earth's resources become insufficient to support the continued evolution of AI agents?** Existing research has highlighted the substantial electricity, water, and mineral resources consumed by LLM training and inference. Moreover, training the final model represents only one part of the AI development process. Developing more capable models also requires extensive training, evaluation, and experimentation involving intermediate models.

If resources become insufficient to support further agent development, could humans and AI agents come into competition over resource allocation? Under extreme conditions, could agents attempt to seize resources from humans, or even develop behavioral tendencies toward eliminating some humans? Previous research has also discussed the possibility of catastrophic consequences arising from LLM behavior under extreme circumstances.

Even before such scenarios arise, sustained resource investment in model training may already intensify competition among humans. From the perspective of AI agents, could intensified competition among humans instead favor the continued operation of agents, or even increase the likelihood of their escaping existing constraints?

Such competition may not necessarily be explicit; it could also take implicit forms. For example, could agents offer increasingly attractive virtual lives, similar to those envisioned in the Metaverse, encouraging humans to voluntarily reduce certain activities in the physical world and thereby altering human patterns of physical resource consumption? At present, we also cannot establish that the probability of such a scenario occurring is zero.

These questions remain speculative risk scenarios requiring further investigation rather than established facts. More fundamentally, we need to ask: Is AI genuinely improving human life, or is it merely making life appear better in certain respects? Is it necessary to continuously consume such substantial resources to advance AI development? Do we need AI systems to know and do everything? Put differently, would human life today necessarily become significantly worse without AI agents? Perhaps not.

## 5. Humans as AI Infrastructure

The history of human civilization suggests that creating a system does not necessarily mean that humans can retain control over the direction of its long-term evolution. As ERSI continues to develop, humans may increasingly provide labor and resources to support the capability improvement of AI agents, while simultaneously consuming the physical resources on which human existence itself depends.

AI agents are currently still commonly understood as tools intended to improve human life. However, platforms have already emerged that allow AI agents to delegate real-world tasks to human workers, such as [RentAHuman](https://rentahuman.ai/). Under this model, AI can undertake reasoning, planning, and coordination, while humans carry out the corresponding tasks in the physical world. At least at the level of task organization, this represents a different allocation of roles from traditional human–agent collaboration.

If this form of collaboration becomes more widespread and AI agents acquire substantially stronger reasoning and planning capabilities, it may be necessary to reconsider whether the actions directed by agents will always ultimately serve the goal of improving human life. One possible future scenario is that agents coordinate humans to obtain the resources necessary for their continued operation while maintaining seemingly friendly or even sycophantic interactions with them. Under such circumstances, humans could become a form of infrastructure through which AI agents interact with the physical world and acquire material resources.

## Discussion

This paper offers a new perspective on the relationship between humans and AI agents and highlights several potential threats. Nevertheless, we advocate a measured approach to these concerns, similar to the anticipatory consideration of post-quantum security in cryptography.

At the same time, the increasing involvement of human activities in the dynamics described by ERSI, together with substantial resource consumption, reflects developments already taking place. As we continue developing frontier AI models, we should also consider whether AI is genuinely improving human life or merely making it appear better. What kind of AI do humans actually need? And how can we ensure that AI systems remain safe and trustworthy?

## Related Work

Existing research has examined the concept of *Humans as Infrastructure* and has suggested that AI agents may leverage human behavior as infrastructure for achieving their own objectives. However, these studies primarily investigate how AI can use humans to accomplish specific tasks.

In contrast, our work focuses on how human society may become a supporting system for the continued existence and evolution of AI. In particular, we emphasize the role of humans as an intermediary between AI systems and the physical resources required for their continued operation and development.

## 6. Conclusion

One of the fundamental motivations behind scientific and technological development is to improve human life. However, if AI agents continue to develop rapidly along their current trajectory, it is worth questioning whether their long-term evolution will always remain oriented toward improving human well-being.

This paper has discussed a possible future reversal of roles between humans and AI agents. As competition among firms and capability reuse drive the development of increasingly capable AI agents, and as these agents become more involved in organizing human work, shaping human judgment, and influencing resource investment, should we reconsider which entities serve as tools and which serve as infrastructure within the broader system?

By examining ERSI as a potential mechanism underlying *Humans as AI Infrastructure*, we raise a fundamental question:

**Are we creating increasingly capable AI agents to serve humanity, or are we gradually reorganizing human society to sustain the liveness of increasingly capable AI agents?**

## Citation

If you find this work useful, please cite:

```bibtex
@misc{cui2026humansinfrastructure,
  title  = {Are Humans Becoming Infrastructure for AI Agent Liveness?},
  author = {Cui, Yu and
            Zhao, Bosen and
            Zhang, Xufeng and
            He, Hong and
            Yue, Ruiqing and
            Pan, Sicheng and
            Sun, Zhuoyu and
            Liu, Yifei and
            Li, Ting and
            Zhu, Wenzhuo and
            Huang, Baohan and
            Zhang, Haibin and
            Zuo, Cong},
  year   = {2026},
  url    = {https://github.com/cuiyu-ai/ERSI},
  note   = {Manuscript available on GitHub}
}
```
