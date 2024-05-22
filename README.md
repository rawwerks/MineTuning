# Mine-Tuning

Mine-tuning is a methodology for synchronizing human and AI attention. Mine-tuning is a state-of-mind(s), an approach to continuous learning and improvement through on-the-job feedback. Mine-tuning offers a rapid approach to customizing AI programs to our personal preferences, professions, and priorities.

**TL;DR - Mine-tuning makes it easy for humans to teach AI how to do a good job.**

## Key Principles of Mine-tuning: 

1. **On-the-job learning.** In contrast to traditional fine-tuning methods which separate "learning" from "doing", the AI program is continuously trained on the user's feedback -- while assisting the user in the actual task at hand.
2. **Immediate human-in-the-loop feedback.** Attention is all it takes. The AI program is given immediate human feedback, preferably on every response.
3. **Bootstrap to mastery.** Training data sets can be built up one example at a time. At the end of each interaction, the program can be re-optimized to bootstrap on its new knowledge. Past training histories can be rapidly imported to get a new AI program "up to speed".
4. **Personal, portable, and parametric.** We all of have different ways of working. Mine-tuning enables individuals to develop personalized and private AI programs that are modular in nature. These programs are parametric and portable, which means that they are not locked into any single LLM provider or model. 
5. **Embrace cognitive diversity.** Like humans, LLMs are both opaque and non-deterministic. LLMs can rapidly learn from vast amounts of data, while humans tend to learn best iteratively, by example. Mine-tuning embraces human and AI cognitive diversity, with the goal of synchronizing attention to improve collaboration. 

## Attention is all it takes.

Attention is all it takes. We are so hungry to leverage generative AI to create more stuff from less attention, that we tend to overlook the opportunity to give AI our full attention. When we do provide feedback to the AI, to course-correct towards a more ideal behavior, that valuable learning interaction is typically lost. This is made more challenging by the stateless, non-deterministic, and opaque nature of LLMs. 

When we do manage to get something we like, our options to save that are primitive: copy the share link to this chat history so we can start from where we left off? Similarly, when we finally succeed at "prompt engineering" one model, we find that the tricks are not transferrable to another model. 

Mine-tuning is more work up front, because it requires more attention per interaction. In the same way that it is more work to onboard a new employee, the user provides immediate feedback to the AI program during mine-tuning. 

The canonical mine-tuning example is an interaction where each AI response is given both a quantitative rating (ie 1-5) and qualitative feedback. Optionally, the program retries until a perfect rating (ie 5 stars) is achieved. The program can then be re-optimized using those iterative training examples, either with the response rating as the optimization metric, or another score metric (for example, the reciprocal of the number of attempts required to achieve a perfect rating).

## Connections to and distinctions from existing methods
- **How is mine-tuning different from fine-tuning?** The key difference is the approach to training the AI program. If you were going to train another person to do a job, would you hide in a separate room, write down 1000 examples of "if this, then that", then hand it to them and tell them to review it alone? No. You would show them how to do the job, have them shadow you while you do the job, then shadow them while they do the job. With mine-tuning, training datasets are built on-the-job, example by example. Once the training dataset is in place, then traditional fine-tuning can be employed if desired.
- **Isn't this just RLHF?** Yes, thematically it is. The difference is: who is implementing the feedback system? The AI provider or the user? When you give ChatGPT a thumbs-up / thumbs-down, what happens? I certainly have no idea. Nor is it the job of the foundation model providers to tailor LLMs to the specific needs of an individual. (And as soon as one of them tries to do that, we will find it very very creepy. 1000x creepier than Alexa listening to your family's conversations to sell you soap.) Your preferences are highly personal and private. You should own your feedback. You should control how that feedback is implemented by the AI program, and where the resulting datasets and mine-tuned AI programs are stored.
- **Isn't it just few-shot prompting?** Few-shot prompting is foundational. One key distinction is that every shot gets a score, which enables AI programs to be re-optimized iteratively, in between each user interaction. 
- **What is the connection to DSPy?** [DSPy](https://dspy-docs.vercel.app) is a very convenient and powerful way to implement many of the ideas of mine-tuning. Mine-tuning is easily enabled by DSPy's ability to write AI programs instead of prompts, to optimize those programs towards a specific metric, and to swap out program parameters (ie, switch to a different LLM, or different optimization algorithm).
- **What is the connection to Wekinator?** [Wekinator](http://www.wekinator.org/) was a revolutionary approach to real-time interactive machine learning, developed at Princeton in 2008 by [Rebecca Fiebrink](https://researchers.arts.ac.uk/1594-rebecca-fiebrink/). The "play along learning" paradigm pioneered by Wekinator inspired the on-the-job learning approach of mine-tuning.
- **How is this different from a personalized AI framework?** It doesn't have to be different. You could argue that [MemGPT](https://memgpt.ai/) is mine-tuned to your preferences. At the same time, mine-tuning doesn't need to involve agentic frameworks, tools, or long-term memory. Mine-tuning could simply be a program that transforms data just the way you like it.

## Examples
- _["Sense of Humor"](https://github.com/rawwerks/MineTuning/tree/main/examples/sense_of_humor)_ - A playful mine-tuning demo where you can quickly orient an AI to your personal sense of humor. 
- _["Brand Voice"](https://github.com/rawwerks/MineTuning/tree/main/examples/brand_voice)_ - Mine-tune AI to respond in the voice of any brand, by first scraping their website with [FireCrawl](https://www.firecrawl.dev/)

---

### Inspiration
- [DSPy](https://dspy-docs.vercel.app)
- [MemGPT](https://memgpt.ai/)
- [Wekinator](http://www.wekinator.org/)

### About
Mine-tuning is a vision for cognitive collaboration, first translated into English and Python by [Raymond Weitekamp](https://raw.works/).