The Hammock-Driven Philosophy
=============================

- Speaker: Rich Hickey
- Conference: Clojure/Conj 2010 - Oct 2010
- Video: https://www.youtube.com/watch?v=f84n5oFoZBc

As mentioned before, this is a more philosophical talk. It is an experience report, not advocacy. There is little methodology or science involved. Reflect on the last time you devoted an hour, a day, a month, or even a year to a single thought. These moments are rare and incredibly valuable. For some, like myself, having the opportunity to contemplate something like Clojure for an extended period is a treasure.

Consider when you last faced a new challenge and felt confident in tackling it. As software developers, we often find ourselves working on repetitive tasks, but the luckier we are, the more likely we will face unique problems. How do you approach these situations without feeling immense risk?

We despise bugs in our programs and strive for quality. We know that fixing issues in the field is costly, so we rely on testing and quality assurance. But is testing during development the best way to prevent bugs?

No.

The least expensive place to fix bugs is during the design phase. Most significant software problems stem from misconceptions rather than implementation issues. Testing and type systems help with implementation defects but rarely address problems of misconception. There are no type systems to tell us whether our ideas are sound or whether our work aligns with those ideas.

### The Importance of Step One

To avoid costly mistakes and ensure the success of a project, focus on the first step. Address misconceptions and thoroughly understand the problem before diving into implementation. Embrace the value of contemplation and thought in your development process.

Analysis and Design may seem outdated and reminiscent of the criticized Waterfall Model, but that doesn't mean the step before 'go do it' is unimportant. Often, we don't dedicate enough time or resources to this phase, which leads to a decline in quality. Let's redefine Analysis and Design as two essential actions: identifying a problem to solve and assessing whether the proposed solution solves that problem.

### Solving Problems, Not Building Features

Software development should be about solving problems, not merely building features. A feature list, even if it comes from the customer, doesn't guarantee that it solves their problem or any problem at all. We must dig deeper to understand the true problem and propose the best solution.

### Problem Solving as a Skill

Problem solving is a skill that can be practiced and honed. Don't assume that only certain individuals are good at problem solving. One resource for improving this skill is Polya's book, ['How to Solve It'], which teaches techniques for solving math problems. While software development doesn't provide mathematical proofs for e-commerce site solutions, the principles of problem solving can still be applied and practiced.

### The Power of Practice

As humans, we become skilled at what we practice. If you practice problem solving, you'll become proficient at it. Ask yourself: would you rather excel at a specific methodology (X) or possess the general skill of solving problems? The choice is yours, but remember that problem-solving skills can provide more leverage in the long run.


### Stating the Problem

To tackle problem solving, first explicitly state the problem you're trying to solve. Far too often, software is built without a clear understanding of the problem at hand. To remedy this, state the problem out loud, discuss it with your team, or write it down. This act of articulation is the foundation of solving the problem.

### Understanding the Problem

The next, and often trickier, step is to understand the problem. Consider the characteristics of the problem that lead to a specific solution space. This stage of problem-solving involves several key activities:

1. **Identify what you know**: Determine the facts, context, and constraints of the problem. These could include customer requirements, system limitations, or other specifications.
2. **Acknowledge what you don't know**: Recognize the unknowns in your problem and contemplate them.
3. **Research existing solutions**: Investigate other solutions to similar problems. Learning from existing solutions can help you make incremental improvements and avoid starting from scratch.

### Documenting Your Findings

While this process doesn't advocate for a specific methodology, it's crucial to document your work in some manner. Recording your findings ensures that the problem-solving process is transparent and easier to replicate or improve upon in the future. Choose a method that works best for you and your team, and make sure to keep track of your insights as you work through the problem.

### Be Critical of Your Own Work

When working on problem-solving, it's essential to be critical of your own solutions. This includes identifying technical errors, logic flaws, and issues of taste, judgment, or abstraction. By scrutinizing your own work, you can address any issues and create a more robust solution. Don't just focus on the positive aspects of your work; seek out tradeoffs and areas for improvement.

### Ask Questions

Recognize that you don't know everything and embrace the unknowns. Ask questions and leave room for inquiry in your problem-solving process. If your documentation doesn't have any question marks, you may be missing a crucial step.

### Seek Diverse Input

To develop well-rounded solutions, expose yourself to various sources of information. This includes reading widely within your field, examining specific cases, and exploring broader related topics. Research papers can provide valuable insights, even if you only understand a small portion of their content. These diverse inputs can help you make connections between ideas and generate more innovative solutions.

### Critique Others' Solutions

While examining other solutions, be critical—even if only in your own mind. Dissecting others' work can help you uncover hidden gems or ideas that can contribute to your problem-solving process. By analyzing and critiquing existing solutions, you can gain insights into how to improve upon them and develop better approaches.

In summary, effective problem-solving requires a critical mindset, asking questions, seeking diverse inputs, and critiquing both your own and others' solutions. By embracing these strategies, you can develop more innovative and robust solutions to the challenges you face in software development or any other field.

### Understanding Tradeoffs

Design is often about making tradeoffs, but this doesn't mean simply accepting the parts of your software that aren't satisfactory. Instead, consider at least two solutions to a problem and evaluate their pros and cons. Documenting these tradeoffs can provide valuable insights as you make decisions.

### Maintaining Focus

When working on complex design tasks, focus is crucial. Computers, while useful, can also be sources of distraction. To maintain focus, consider stepping away from your computer or finding a quiet space, like a hammock, where you can concentrate without interruption. Recognize that intense focus may result in temporarily neglecting other tasks or communication, and let those around you know that this isn't a reflection of your feelings towards them, but rather a necessity for the task at hand.

### Utilizing Waking and Background Minds

Effective problem-solving often involves using both your waking and background minds. Your waking mind is analytical, tactical, and focused on short-term decisions. However, relying solely on this aspect of your mind can lead to finding only local maxima, rather than discovering more optimal solutions.

To fully harness the power of your mind, assign tasks to your background mind during your waking hours. This can involve thinking deeply about a problem or engaging in focused activities that provide your background mind with work. By doing so, you can enhance your problem-solving skills and come up with more innovative solutions.

### Waking Mind: Analyzing and Critiquing

Your waking mind is excellent at analyzing and critiquing ideas, even those that initially seemed brilliant. This aspect of your mind is useful for identifying potential flaws or shortcomings in concepts that your background mind might have generated.

### Background Mind: Synthesizing and Strategizing

The background mind, although not limited to sleep, is most accessible during rest. It excels at making connections, synthesizing information, and devising strategies. For example, creating abstractions or designing programming languages requires strategic thinking, which is a strength of the background mind. To come up with innovative solutions to non-trivial problems, it is crucial to engage this aspect of your mind.

### Sleep: Sorting and Solving

According to Scientific American, sleep is essential for processing daily information, reinforcing memory, and sorting through the input we've gathered throughout the day. Evolution has equipped us with the ability to find hidden relations and solve problems during sleep. However, to benefit from this, it is necessary to think deeply about a problem while awake, assigning it as an agenda item for your background mind.

### Feeding the Background Mind

To fully harness the power of your background mind, you need to work hard during your waking hours. Invest time in thinking about a problem, analyzing requirements, reading relevant materials, and examining competitive solutions. This effort will provide your background mind with the necessary input to work on the problem and come up with innovative solutions during periods of rest.

### Writing Down Problem Components

When faced with complex software problems, our working memory (with a limit of 7 +/- 2) often struggles to handle the numerous components involved. To address this, write down every aspect of the problem, constraints, and potential solutions. This helps create a comprehensive agenda for your background mind to process.

### Surveying Your Notes

Once you've written everything down, survey your notes to help load the problem into your mind. By examining your written material, you can juggle multiple aspects of the problem simultaneously, much like juggling different colored balls with the help of an assistant.

### Mind's Eye Time: Reflecting Without Input

After surveying your notes, it's crucial to step away from the computer and engage in quiet reflection. Close your eyes and visualize the problem in your mind's eye. This "mind's eye time" allows you to shift from input reception mode to a state of contemplation and recall. By doing so, you exercise your ability to bring various problem components in and out of your mind, making them more likely to become agenda items for your background mind to work on.

### Give Your Brain Time to Work

When trying to find a solution to a complex problem, it's important to allow your brain enough time to process the information, especially during sleep. Even if you feel confident about your ideas, it's best to sleep on them for at least one night. Sometimes, though, overnight might not be enough, and finding good abstractions or satisfying multiple constraints can take longer.

### Work on Multiple Projects Simultaneously

To deal with the need for more thinking time, try working on multiple projects but focus on one project each day. If you find yourself stuck on one project, switch to another one for a few days. This method can help you avoid getting hung up on a single problem while still giving your brain time to process different issues.

### Evaluating Your Ideas

Once you've come up with a potential solution, you'll need to analyze and evaluate it to see if it's actually a good idea. Sometimes, the solution might not be related to the problem you were currently working on, but that's okay. Capture the results and switch to the relevant project to take advantage of the idea.

### Implementing Your Solution

After evaluating your ideas, you'll eventually need to implement them by coding. It's essential to strike a balance between thinking and typing to ensure that you're solving the problem effectively. A compact and well-thought-out solution is often a strong indicator of a good idea. Remember, knowing your challenges and working on them is a positive approach to problem-solving.

### Gaining Confidence in Your Process

By following this problem-solving process, you should gain confidence in your ability to come up with effective solutions. Even if you've never encountered a particular issue before, trust in the process and the solutions you've come up with after adequate contemplation.

### Iterative Problem Solving

It's crucial to understand that problem-solving is not a linear process. You may need to test your solution, gather more information, and iterate on your initial ideas. This doesn't mean you're following the Waterfall Model; rather, it acknowledges the necessity for continuous learning and improvement.

### Accepting and Learning from Mistakes

Understand that you will occasionally be wrong or come up with better ideas later. This is a natural part of the problem-solving process and a sign that you're still growing and learning. Don't be discouraged by changing requirements or new facts; instead, adapt your solutions accordingly and continue refining your approach.

### Embrace Fearlessness

In conclusion, don't be afraid of being wrong or making mistakes. The key is to learn from these experiences and improve your problem-solving skills. There may not be a concise summary for this approach, but the underlying message is clear: trust in your process, adapt to new information, and never be afraid to make mistakes.
