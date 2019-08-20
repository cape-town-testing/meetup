# Cape Town Testing Meetup - Q3 2019
## Notes
#### Talk 1: Team Psychological Safety – Brian van Vuuren
##### INTRO
* Daily commute from Stellenbosch to Allan Grey
* New role / new position as a Frontend Developer / New friends / New life
* Hit someone in the road on daily commute – devastation
* Received phone call for a new job offer – remote consulting work, better salary, no driving
* “Have to take this job”
* Communication re:new job was staggered and slow, person in communication was high-up so responses were slow
* 1.5 month later = things have changed
* Didn’t want the new job anymore – wanted to stay and work with current team / didn’t want to leave
* Why?
* <Brian to provide team dynamics/psychological frames of reference>
##### WHAT IS IT?
* Belief in others / no punishment
* Deep sense of trust
* Raise issues / call them out before damage is caused
* Soft skills
    * “Devs are the soft stuff” even though they don’t like / deny it
##### WHAT IT IS NOT…
* Environment where everyone loves everyone, and no one makes mistakes
##### KNOWLEDGE ECONOMY & PSYCHOLOGICAL SAFETY
* We live in a knowledge economy made up of:
    * Knowledge
    * Friction
    * Competition
* Psychological Safety allows us to co-exist in this environment to deliver as a team/business
    * Not restricted to work, also relates to family/outside of work relationships / social circles / people
    * Can’t avoid it
##### CHEMICALS IN OUR BRAIN
* Selfish Chemicals
    * Endorphins – feel good chemical - essential to survive (hunting buck example)
    * Dopamine – goal achieving / addiction chemical
* Selfless Chemicals
    * Serotonin
    * Oxytocin – physical touch required / love / relationships chemical
* So, do we need to lookout for ourselves or others?
    * Both
    * 4 chemicals together are our core drivers as humans
##### CIRCLE OF SAFETY
* Iron age man example
    * You look out for me, I look out for you – more people = increase our chances of survival
* You do this for me, I’ll do that for you – by working together with trust / cooperation
    * Need to foster this environment and prove everyone reciprocates what they receive
* Many concerns/threats exist to us in the tech industry
* Placed in a team = safe space where leader looks out for you
    * Decreasing your worry of threats
    * Increase your productivity
    * Leader controls what they can to minimize fear “I have your back if you have mine”
* Pandora bracelet example
    * Mother-in-law – wants cream not brown
    * Shop assistant unwilling to cooperated/provide good customer service = unsafe environment, only concerned about protecting herself
* Need to have room to do your best
##### HIGH PERFORMING TEAMS
* Able to speak up / contribute
* Able to pick up on non-verbal cues
* At Google – their success is based on:
    * Talking
    * Intuition 
* 2 things that matter most when building relationships is building connections / talking and intuitively knowing how others are feeling
* Acknowledge headspace/support of others and don’t let others get away with things if they’re going through a tough time
##### CLOSING
* Gallop survey – showed decrease in accidents/mistakes 
    * But in an unsafe environment mistakes are hidden
    * In a safe environment errors/mistakes increase because fear of reporting them is reduced
* Important skill – be open to being challenged
    * Conflict = collaborator
    * Fight vs. Flight inherent 
    * Conflict = brain has abandoned you = biological response
* Most people are risk averse these days
    * Flip a coin – we would rather not lose vs. win
    * Don’t want to be proven wrong
* Blood = thicker than water
    * Doesn’t refer to family but those who you have shed blood, sweat and tears with
    * Stayed at Allan Gray because of the bonds built and the circle of safety
* Team needs to put in the effort, and someone needs to champion for this concept
* You want people to say “I know they will do it for me”
##### QUESTIONS
1.	What can we do in the workplace to promote this to the CEO for top down infiltration?
a.	Answer: Not a 1-man band, need to get more people on board. Don’t start at the top. Let it bubble up from the bottom.

# Talk 2: Data Migration and Data Warehouse Testing – Francois Marais
* Busii – pronounce “busy”
    * Financial Services / local bank / 5years loyalty program testing
* diffst = inhouse dev tool
    * build your own?
* Keep talk high-level due to client confidentiality
* POS = source DB / Rewards = target DB
    * Data is read from the source
    * Then transformed
    * Stored in/read from the target DB
* Loyalty Program example
    * Source data = millions of rows & 1000s of business rules to work out rewards
    * Very NB to test accurately because customers scrutinize this data / their rewards
* Comparing individual data items = hard to automate 
    * Use SQL client and compare source/target
* Coverage issue can be resolved by:
    * Aggregated SQL 
        * Bug life cycle = more complicated
    * MINUS Queries
        * But this is slow
* When testing we:
    * Look at a few rows at a time
    * Look at a few columns at a time
    * Look at all data to find discrepancies
* Not humanly possible to look at millions of rows of data = need for testing tools
* In-house solution was born - diffst
    * YAML text file
    * Run test case with business rules against the source/target
        * Use snippets to create test data
    * Report on deviations in column orientated output
    * Positive result = 0 deviations returned
    * No VMs required per environ
    * Faster bug life cycle because you can show which test cases/business rules applied found the discrepancies
QUESTIONS
1.	What is your SQL strategy / what are the bottlenecks?
a.	Answer: Uses GO. Tool goes directly to data warehouse and you can setup configurable batch sizes.

2.	Does the tool transform data from PROD to non-PROD environ and does it support DB2?
a.	Answer: No transformation of data. Yes, it supports DB2.


