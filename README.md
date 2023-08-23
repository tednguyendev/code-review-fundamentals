## [Reviewing Pull Requests](https://chelseatroy.com/2019/12/18/reviewing-pull-requests/)
- Code reviews: we know they [make our code better](https://blog.codinghorror.com/code-reviews-just-do-it/). _How_ do we do code reviews? There’s less agreement on that.
- We have, in pairing, an _expectation_ is that the pair will _participate in implementing_ any alternative that they suggest.
- In fact, the state of pull request quality is _so bad_ that most advice I’ve read on how to do a good review _only_ addresses the idea that you shouldn’t insult someone’s code.
- They’re bad because they are delegating responsibility to the original developer to do both the feasibility test and the implementation of those ideas.
	- They’re recording their idea in such a way that they get credit if it works out, but the original implementer undertakes all the risk that it doesn’t.
- Heretts the proof that pull request reviews could be extremely effective: they are still sometimes useful, even when they are this bad. So why do we do them this badly, when there is so much potential for them to change our code for the better?
- If the reviewer lacks sufficient context to modify the code themselves, the pull request has failed on the goal of context transfer.
- My review should save time and frustration, not create it.
- The fact that this takes so much time illustrates precisely why pairing is efficient. There is immediate context transfer between two people working together
- A reviewer spending this time is still a better use of resources than having the original developer chase down solutions suggested by lazy, delegating commentary on their pull request.
- I spend time asking questions. I want to have full context on this code.
- Points out what's working and what's not, and links to documentation where useful.
	- Highlights laudable work by the original developer, and asks questions before making assumptions or judgments.
	- Explains the reasoning behind suggestions, whether that reasoning affects functionality or adheres to convention.

## [Code Review: Best Practices](https://app.pluralsight.com/library/courses/code-review-best-practices/table-of-contents)
- Code Reviews amplify the good and the bad of a team
- CR is a mix of hard skills and soft skills
- Average numbers of code review ppl required: 2
	- And at least 1 should know some biz logic
- When review code than you are not sure(or u are junior)
	- CR is also about knowledge sharing
	- CR is also about mentorship, but the author should not spend so many time teaching on the PR
		- Have another sharing session
- It's not ur code
	- It's the team's code. Once the PR is merge, the team have to have responsibility and maintain it
- The bigger a PR, the longer it take to review, and the more merge conflicts it will have
- Prefer adding comments into the code than add PR comments, as PR comments is less visible
	- But can do PR comments in cases like:
		- As discussed with John, we decided to implement it like this because...
- Avoid words like "you" to attach the ego of the author from their code. Consider "I", "we", or "the code"
- OIR rule
	- ![](Attachments/CleanShot%202023-08-23%20at%2012.27.00%402x.png)
	- Help to skip request for clarify
	- Promotes learning
## [RailsConf 2015 - Implementing a Strong Code-Review Culture](https://www.youtube.com/watch?v=PJjmw9TRB7s&ab_channel=Confreaks)
- Ppl only think abt Code Review as finding bugs
- Other good things
	- Knowledge transfer
	- Team awareness
	- Alternative solutions
- CR is just discuss ur code with ur peers
- Normal, we talk abt abstract things, pattern. In CR, we go into details.
- Rules
	- As an author, provide context
		- Context is god
			- Author need to give a lot of context
			- Beside being not able to review, not have enough context also make it confusing, boring, and hard to learn things from. So no, bye review.
			- Work a task for 3 days, it's totally worth spend some more minutes giving context to the PR
	- As a reviewer, ask questions rather than making demands
		- Ask, don't tell
			- Don't command
		- Don't use "just"
			- "Why did't you just ..."
- Can have a list of things on everytime review
	- ![](Attachments/CleanShot%202023-08-22%20at%2014.42.30%402x.png)
