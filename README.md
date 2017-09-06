Mind dump for my favorite software development practices, rules of thumb and quotes.

## Clean code

- “Any fool can write code that a computer can understand. Good programmers write code that humans can understand.”
- Focus on readability (for a sake of other team members), not on perfection.
- "If something is too big for your head you cannot reason about it"
- Minimize 'Cognitive Load' - thinking too much over a simple thing.
- "See what's really there" - if there is an inconsistency:
    - it may be a special case
    - if it's not then it should be a sign that something went wrong
- Familiarity is not simplicity:
    - you get used to crappiness
    - crappiness is bending your brain
- Sometimes it is worth to step back one step and ask yourself: "What's the dumbest thing you see?" (or ask this question to someone else)

- Complexity is the default state - it grows one day at a time
- Consistency at scale is a daily choice - agree on idioms and guiding principles
- Strive for simplicity - choose tools and techniques that make it easier because "it really shouldn't be this difficult"
- Simple design is not stupid design

- YAGNI:
    - don't commit early unless you know you are going to need it
    - think about event horizon - how soon the dumb thing you did is going to be irreversible
- Push often and commit often - [make the sausage](https://sethrobertson.github.io/GitBestPractices/).
- If you have generic repositories it means that you need a Query
- Be DRY until it starts to trouble you
- DRY can stiffen your code (the bad way)
- "It looks the same but it's not the same"
- "I wasted time perfecting and complicating a straightforward module so that you could waste your time understanding it"
- "If you only have a hammer, you tend to see every problem as a nail"

## Frameworks

- "The framework cannot know how to separate your concerns for you. It should only provide powerful, expressive tools for the user to do it correctly."

## Testing

- Initialize only what is necessary to make the test pass
- Use fluent api / builder to build complicated objects
- **Tests are communication tools**
- **You should still think when writing the tests**
- Write test instead of debugging
- Clean code principles also apply to tests
- Frameworks can be wrapped to make them testable
- Fake it till you make it
- Use business vocabulary everywhere, even in the unit tests

## Debugging

- "If you're good at the debugger it means you spent a lot of time debugging. I don't want you to be good at the debugger."

## QA

- **QA should prevent bugs not find them**

## Design patterns

- Do not make new problems only to solve them by applying design pattern
- Singleton is OK if it does only one of those two things at a time: reading or writing
- Strategy and factory patterns are the best friends
- Inject strategy by DI unless it needs to be changed often. Then use factory.
- Decorators can be done by using aspect programming.
- Do not use decorator if it changes completely the behavior of decorating object.

## SOLID:

- Liskov - if you surprise developer - know that something bad happens.

## Architecture

- I define architecture as a word we use when we want to talk about design but want to puff it up to make it sound important
- Making something easy to change makes the overall system a little more complex, and making everything easy to change makes the entire system very complex
- Shift mindset from fail-safe design to safe-to-fail experimentation
- Find at least one alternative
- Coupling is the biggest thing that causes fear

## Planning

- Hofstadter's Law: It always takes longer than you expect, even when you take into account [Hofstadter's Law](http://en.wikipedia.org/wiki/Hofstadter%27s_law).

## Improvement

- Read code
- If you put yourself in the way of unusual experiences you may discover that there are things you really enjoy
- The better you understand what you are doing, the better you will do it
- "I was a lead dev so I did couple of code review more than the others"
- Fake it till you make it
- Give and get feedback often (it's like commit often but with people)
- Communication is like a driving car - you don't want to cause an accident
- If you want to master something you need to teach it
- You should be spending your time building stuff, not studying for multiple choice tests
- "Nobody wants developers to reinvent the wheel (again), but reading about how a wheel works is a poor substitute for the experience of driving around on a new wheels of you own creation"
- Optimize for team productivity
- Choose a team where you are the worst of them
- Find a mentor, be a mentor

## Open Source

- Put initial version on-line
- "No contribution is too small"

## Other

- Java and .Net have been designed to survive enterprise development
- Brilliant software engineers will follow bad plans put forth by people in power
- All code (production, tests) is a technical debt

## [The Zen of Python](https://www.python.org/dev/peps/pep-0020/)
- Beautiful is better than ugly.
- Explicit is better than implicit.
- Simple is better than complex.
- Complex is better than complicated.
- Flat is better than nested.
- Sparse is better than dense.
- Readability counts.
- Special cases aren't special enough to break the rules.
- Although practicality beats purity.
- Errors should never pass silently.
- Unless explicitly silenced.
- In the face of ambiguity, refuse the temptation to guess.
- There should be one -- and preferably only one -- obvious way to do it.
- Although that way may not be obvious at first unless you're Dutch.
- Now is better than never.
- Although never is often better than *right* now.
- If the implementation is hard to explain, it's a bad idea.
- If the implementation is easy to explain, it may be a good idea.
- Namespaces are one honking great idea -- let's do more of those!
