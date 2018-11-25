# 2. "Automation In Sprint" | 2018-Q4 Presentations
## Shekhar Ramphal

1. End up running with man down in team; full stack team - need db, ui, etc.
2. CI brings own challenges
	1. Hours of overtime to retro fit tests
	2. Testing becomes the bottleneck - happens at standup almost every other day
3. Ratios are wrong!  There are not enough testers to match the number of devs
4. Not every team has a tester thats automation skilled - don't know how to write automation tests; steep learning curve
5. Testers have to put extra time in to keep up with devs
6. Tester code is being reviewed harshly (position of comma, 1000s of lines of comments)
7. We have to change the way we work to adapt to in-sprint automation.  What should the testers be doing?
8. Some testers move away from writing automation tests altogether
9. Might be difficult to change to pair programming when the organisation isn't used to working that way
10. Develop a common language across dev and testing - learning curve for us testers (maybe devs can "dumb down a bit")
11. We are inquisitive by nature - so poke the devs to learn the technology
12. Mini waterfall sprint - all the dev upfront and a few days to do tests - this results in stress!
13. How do we get involved earlier?  Spend time looking at code reviews, pull requests.  If you know the code, can test less and more accurately
14. Remove the bulky test tooling - e.g. selenium, qtp, etc.  So many dependencies.  I've set this up, its great, lets use it.  It doesn't work if only the testers can use it (key man dependencies)
	1. Got to be tools that the devs are also willing to use
15. Takes a programmatic approach - use languages and tools that the devs also use
16. Moved the test code closer to the production code - don't limit yourself to only being able to run overnight
17. If closer to the dev - then runs with the builds - forces the devs to get involved to fix the code so the tests will pass
18. Test code is not feature code
19. Dry concept of code - don't repeat yourself. Keep it clean - don't abstract like devs - makes it easier to debug tests
20. Don't bombard juniors with heavy comments on tests - will discourage them
21. Tester have attachment to code - only I can fix and maintain the tests... This is contrary to the way developers work.
22. As tester, must also write tests so that others can maintain.  If you don't, you miss the boat then
23. Learn to context switch - kind of hard for testers to do... but necessary to be able to cover all the components of the system
24. Have an SLA for build pipeline to take less than 10 minutes.  End to end tests will take too long 
	1. Doesn't help when tests take overnight to run.  Take too long to run really good tests for such a short tests.  Who checks the issues?  We have a guy!  It takes him another hour to check... and then there was an environment problem so we have to run again
25. __QA don't be quality assurance__ - be a quality advocates.  Much better to have a quality goal.  Driving the culture with the devs to improve quality in the team
