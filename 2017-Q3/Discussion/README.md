# WORKSHOP: 
EXPLORING THE ROLE OF TESTERS FROM AN ORGANISATIONAL POV: A REVOLUTION OF TESTER COMPETENCY
## INTRO AND CONTEXT:
IAN & ISMAIL FROM ALLAN GRAY PRESENTING.
PROVIDED ALLAN GRAY CONTEXT:
-	MEDIUM/LARGE FINANCIAL FIRM
-	IN EARLY DAYS AS RELIANCE ON IT SYSTEMS INCREASED, RESPONSIBILITY FOR DEVELOPMENT & DESIGN RESTED PRIMARILY WITH BUSINESS STAKEHOLDERS
-	IT TEAMS PRIMARILY FOCUSED ON MAINTAINING SYSTEMS
-	LARGE NUMBER OF LEGACY SYSTEMS – DEVELOPED WITH LIMITED TESTING
-	IN MORE RECENT YEARS, SHIFTING FOCUS INTERNALLY & EXTERNALLY
-	SHIFT TO THINKING ABOUT BIG CATEGORIES OF SYSTEMS
-	FORMING STRONG TEAMS OF BOTH BUSINESS STAKEHOLDERS AND IT STAKEHOLDERS TO BUILD/IMPLEMENT SYSTEMS SOLUTIONS.

# THE WORKSHOP:

Three focus groups, each allocated a context in the form of a type of software solution to be implemented:
1.	Brought In House & Shared Source
2.	Vendor Product – Closed Source
3.	Custom Software

## FEEDBACK 1) Vendor Product – Closed Source:
Top Problems of the Context:
1.	Misaligned Priorities
2.	Incorrectly estimated solution based on Sales Pitch
3.	Missed requirements/scenarios
4.	Time consuming change management
5.	Indirect communication loops
6.	Tech & Business Integration
PREVENTIONS, CURES AND LEVERS:
1.	Impact Analysis with correct people involved.
-	Understanding the assignment
-	Understanding the risks
-	Understanding the scope & responsibilities
2.	Strong Initial Communication and Engagement with Vendor
-	Relies on strength of relationship between business stakeholder & tester.
-	Strong internal communication and engagement means less chance of Problems 1 & 3 occurring.
-	Role Play the vendor meeting
3.	Involve DevOps early to set up infrastructure.
4.	Fly a team member(s) to the vendor site for context and relationship building.


## FEEDBACK 2) Brought In House & Shared Source:

1.	Is difficult/ Tricky to deploy
2.	You lose support if code modified
3.	Absence of contextual knowledge of code base
4.	Lack of version control/ configuration  management 
5.	You only get code from vender but no test scripts 
6.	Cascading breaks
7.	Lack of testability 

Things to consider when using vender software

1.	Take time to understand the code base
2.	Plan for product support 
3.	If automated -  budget for time


## FEEDBACK 3) Custom in-house built Software:
### Problems / Symptoms / Warnings

New technology requires a shift from a critical to learning mindset

•	In “learning mode”, functional issues more likely to slip through so testing and development quality is negatively impacted

#### Ideas / Preventions / Cures:

•	Make a decision to have team members or teams in the org to do this

•	Acknowledge the costs and get buy in from business

•	Allow the learning to get to a logical end point so that efforts in training are not wasted

•	Mentorship between ‘experts’ and testers taking on the skills is important

•	Spotify style guilds in the organization can be a strong support network


### New technology may require testers to move from manual testing to writing code to test

•	Learning mindset scenario once again

•	Focus shifts to how to write the test rather than how to test – may result in degrade in quality, especially missed edge cases
#### Ideas / Preventions / Cures

•	Cooperate with developers and empower them to build tools that helps testers write tests.

•	Reduce the time from getting skilled to being productive through pairing with a developer.

•	Learning by doing real tangible uses cases which need to be built brings the learning home and helps with reconnecting with the critical thinking.

When developing in-house, need to worry about continuity and how to retain knowledge when people leave
•	How do we ensure documentation stays up to date?
Ideas / Preventions / Cures
•	Keep documents small and context-specific.
•	Try keep as much information as possible in the code and tests so that the software is self-documenting
•	Test self-documenting code by asking people with limited exposure to the module to explain what it does based on the tests and the API documentation.

### Picking the technology to use and deciding on “the right way to build” can take a long time when building from scratch

•	Often make use of prototypes to prove/disprove assumptions – throwaways 

•	People have to learn enough to build and test prototypes and if tech keeps changing, then this requires relearning over and over

•	Need business buy-in because it takes time to upskill, choose the tech and only then build the feature.

#### Ideas / Preventions / Cures

•	Hire in experienced and knowledgeable people to help pick the solution faster

•	Use an off-the-shelf product rather than building something from scratch can expedite delivery but rigorous evaluation of the what the software provides in respect to what your organization needs is critical

•	Building out tooling to provide the capabilities you require is costly and takes time but allows you to build it to exactly what the organization needs.

•	There is a danger that if it takes too long to build out the tooling you are left with something that fits stale capability requirements


### If you’re working with cutting edge technologies, then the skills are usually scarce, so there are concerns around

•	Retaining the skilled people you already have

•	Finding new people which are scarce and probably expensive

#### Ideas / Preventions / Cures

•	Hiring in skills is incredibly difficult and should not be downplayed

•	Retraining has to be bought into by the organization and by the teams.

•	Change management effort is high especially if you are moving from an existing well known technology stack to a completely new technology stack.

•	There is a danger that cutting edge technologies can fade quickly 

### Working as large a group on a large product

•	Slowed down by others working on top of each other / close to each other

•	Things breaking unexpectedly after change

•	Teams doing similar work and not knowing about other efforts
#### Ideas / Preventions / Cures

•	Break down big system into smaller independent modules

•	Take business through every module

•	Test every single module

•	Rewrite rather than fix issues

•	Code reviews

•	Smaller teams with increased focus

•	Have a test plan that one can work through systematically

•	As a new section/component works, then shut down the old one

•	Document modules for others to understand what the module does

