# AI Adoption Process for Skeptical Engineers
From my experience, senior-leaning engineers tend to be more skeptical of the outputs of AI tooling, particularly if they only assessed early models and tools before writting them off entirely. For good reason too; [it can be faster to rely on individual experience](https://arxiv.org/abs/2507.09089) to get things done. 

**Old Hypothesis**: If we assume distrust in the quality of output as the blocker for developer adoption, then wouldn't the problem solve itself once the tools become better? 

The outputs have improved since mainstream experimentation in the world of enterprise engineering, but there's still a significant amount of resistance to adopting AI enabled workflows. 

**My Hypothesis**: While AI dev tools are easy to onboard and set up, adoption is difficult because the skills and capabilities of AI can be misunderstood as a loss of control, craft, and discretion for individual engineers. For a senior engineer, the feeling of lost autonomy, the association with poor output quality and the pressure to adopt tools that they don't believe adds value, is incongruous with their professional (and maybe even personal) identities as a software engineer: a knowledgeable problem solver who builds great products.

To facilitate the adoption of AI developer workflows with skeptics is to build geniune adoption through respecting engineering judgement, demonstration, experimentation, and supporting engineers as they navigate the biggest industry shift in recent history. To mitigate fear and apprehension, a user-first approach must be taken to address objective and subjective concerns.

> Note: I believe that this plan needs to be executed at the team level, not the individual level, even if individuals are skeptics. It's important to establish the team environment as optimistic and data-driven, rather than continue to single out skeptics.

## Phase 1: Understanding & Addressing Concerns
### 1.1 Conduct Individual Conversations

Hold 1:1s with each engineer to understand their specific concerns. Document themes without judgement, as they will often be systematic issues. Some themes I've experienced through research include:

- **Quality concerns**: "AI generates buggy/insecure code"
- **Craft concerns**: "I'll lose my skills or become dependent"
- **Workflow concerns**: "This will slow me down, not speed me up"
- **Trust concerns**: "I don't understand what the model is doing"
- **Intellectual property concerns**: "What happens to our code?"

I've found it especially helpful to have a "rant session" where engineers share with me any irritations they experience during the SDLC, no matter how large or small. We then find ways to use AI to remove or lessen these irritations. For example, writting good commit messages.

### 1.2 Set Transparent Expectations

Share with engineers explicitly how you expect them to utilize AI:
- To increase unit test code coverage by generating more test cases
- Making frontend code accessible to WCAG 2.1 AA standards
- Speed up code reviews

Also share what your expectations are not:
- Don't use AI for everything
- Don't stop reviewing code entirely
- You do not have less autonomy now

It's also important to align these expectations to the business context and to affirm where the organization stands with AI tooling, but looking to them as SMEs to evaluate the best ways to utilize AI skills and capabilities.

### 1.3 Share the Research
Provide real annecdotes on how experienced engineers internally have used AI tools effectively with demos, a prompt library, templates, and spike findings. The focus needs to be on how engineers can use AI to think creatively, catch gaps in logic, meet a higher standard of quality, and reduce context switching **faster**, not on the quality of the code output.

## Phase 2: Low-Risk Experimentation
### 2.1 Commit as a team to spend one week using AI in a new way in their worfklow.

Push the team to commit to using AI in new ways in their workflow for an explicit timeframe as an experiment. Bake it into the team process (e.g. Jira stories in the sprint with allocation) and discuss in team retro. If there's broader team or department support, make it a fun competition. The group who comes up with the most number of use cases for using AI in engineering workflows wins [insert highly valuable prize here - team lunch? merch? a big trophy and bragging rights?].

### 2.2 Collect feedback during daily standup
Assuming the team meets daily, include the question: "how did you use AI yesterday?". This sets up group accountability and a medium for knowledge sharing. Verbal feedback is also easier for the contributors, so managers can take notes to systematically collect feedback daily.

## Phase 3: Analysis and Iteration
While some recommend doing A/B tests to validate output quality and speed when using AI tools versus when not, this is irrelevant to the larger goal of increasing AI developer tooling adoption. **If they are more efficient with AI tools, it won't matter if they don't/won't use it at all.** This phase is focused on removing friction in the developer experience so that using AI becomes second nature.

### 3.1 Host team retrospective
- What worked well? What didn't?
- Which tasks benefited from AI? Which didn't?
- What concerns were validated? Which were resolved?
- What best practices emerged?

Celebrate both successes and constructive failures.

### 3.2 Make Adoption Opt-In by Task
Don't mandate AI tools globally. Instead:
- Engineers choose when AI tools add value to their specific context
- Teams decide which workflows benefit from AI assistance
- Individual engineers maintain autonomy over their development process

The goal is to make AI tools a valuable option, not a requirement. Adoption of these tools need to be regularly assessed. This can be done systematically by including in 1-1s a section for discussing AI in their workflows.

### 3.3 Regularly and Publically Celebrate Wins
Shout out effective uses and new ways of using AI that the team discovered. Experiment yourself and share your findings. I have a monthly meeting with my teams where we chit-chat on all the latest happenings in the tech industry, and we often discuss ways we're using AI in our professional and personal lives. 

### 3.4 Codify What The Team Agrees On
Did everyone agree that using AI made it super easy to meet the code coverage thresholds? Fantastic! Codify it within the team handbook (or wherever it's documented) as a formal process. This solidifies AI in your team's workflow, builds momentum, and sets accountability. It is also a precedent for anyone onboarding that the expectation is for the entire team to use AI in the workflow in the defined ways.

## Phase 4: Determine if Expectations are Being Met
It's not guarenteed that this process will win over everyone, but it is a gradual, less disruptive approach to establishing an expectation to how the team operates. When given enough notice and support, clear expectations, opportunities to share feedback, and agency to learn and contribute, I believe that growth-minded engineers will rise to the challenge. When these expectations aren't being met, there may be something more personal at play. At this point as a manager, the discretion lies in how to support your team member (within reason) and when to determine that this environment is no longer conducive to their growth and the success of the team. Given that the whole industry is moving forward in this direction, an engineer who is still skeptical at Phase 4 will likely struggle in any engineering environment outside of their current one.

## Success Indicators
Because we're experimenting with ways to increase AI adoption and not measuring the quality of output or productivity levels, these success indicators lean more subjective and qualitative (but could also be more objective and quantitative; depends on how much effort leadership wants to put into this initiative):

✅ Skepticism evolves from "I don't trust this" to "This works for X but not Y"  
✅ Engineers report reduced time on low-value tasks (tests, boilerplate, docs)  
✅ Code review quality remains high or improves  
✅ Engineers voluntarily share AI tool tips with each other  
✅ Engineers feel empowered to choose skills that fit their needs  
✅ Team velocity increases on well-defined tasks  
✅ Engineers report more time for design thinking and problem-solving  

## Red Flags

On the contrary, these are signs that the plan isn't working well. Note: given Phase 4, these signs are concerning when more than 1 engineer experiences it.

🚩 Engineers feel pressured to show adoption for performance reviews  
🚩 Code review rigor decreases because "AI generated it"  
🚩 Engineers stop learning fundamentals or debugging skills  
🚩 AI-generated code gets merged without understanding  
🚩 Skeptics disengage rather than voicing ongoing concerns  
🚩 Tool usage becomes performative rather than genuinely helpful  


## Dependencies
The biggest dependency is a commitment from the engineering manager. Not only to increase AI adoption, but to prepare their engineers (indivudally and as a team) to shift to a new paradigm of working. Without both, the team will lag behind and collaboration will erode. The manager needs to balance being optimistic and pragmatic to meet the organizational goals, regardless of their personal opinions. At the end of the day, a manager shouldn't dictate how the team builds, but to enable and support their team to accomplish goals and solve problems.

# Conclusion
The goal of this plan is to help your team move faster by giving them effective tools and the autonomy to use them wisely. Skeptical engineers who discover genuine value will become your strongest advocates. This cannot be accomplished by forced adoption. Instead, it requires building trust through transparent experimentation and respecting engineering judgment.
