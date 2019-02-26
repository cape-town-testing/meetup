# 2 "Join the final revolution in functional testing"

# Ben Harper [@rogojin](https://twitter.com/rogojin)
* OneTwoTest - something he's been working on for a few years
* You can contact him at Ben@OneTwoTest.com
* OneTwoTest is a new tools for functional regression testing of web apps
* Good progress over the last two years - but working in a vacuum
* Looking to the community to help him make it better
* Tool looks only at the pixels of the application.  No XPath or CSS DOM selectors
* Why has noone done this before?  We didn't know how.  Only recent advance in AI have made it possible
* The application is live to sign-up... its free for now - go sign up
* Pricing will be based on the number of tests, not on the number of people that have access
* Showed demo of application
* Need to use Chrome browser to record test (only chrome has the necessary extension)
	* Allow incognito mode (i.e. a clean sandbox)
* Playback allows you to scroll through the test or move between discrete events (e.g. mouse clicks)
* Test exection will take about as long as the real execution did
* Demo included showing how comparison of Actual vs. Expected looks when a test failed
* How does AI fit into this picture
* AI can mean many things
* One example is a self-driving car - taking inputs from the pixels of its cameras to figure out what is a car, a road sign, a pedestrian
* Once its figured that out, passes it on to a regular logic programme to decide on the response (i.e. brakes, spead up)
* Another example is alpha-star - an AI developed by Google to play the game starcraft
* The job of the AI is to figure out what the next move is based on events
* Self-driving car might be eyes whereas the alpha-star is more of a brain making decisions
* Trying to accomplish this with OneTwoTest - the AI is the eyes, but backed by a more convention brain-type programme
* Does AI deserve the buzz?  Yes - showed performance of the winning system on image NET
* The job of the AI is to figure out whats in a picture.  People have been trying to build these programmes for a very long time.
* In 2012 was the first massive drop with deep learning, but then it plateaud until in 2015, it was able to beat humans for recognition
* How does OneTwoTest see the world?
* Detect all text using OCR... memorise the text and then erase it.
* The next step is to detect all areas - feature points that have a specific signature / fingerprint for comparison with each other
* Once the feature points are identified, the text is added back as virtual feature points (seems to be based on phoenetics - A in cat is different to the A in ball)
* When comparing actual vs expected, these feature points are compared
* Ben showed a graphical depecition of the decreasing maintenance cost with increasing system intelligence (joked about how scientific it is)
* Humans need much fewer instructions (they fill in the blanks)
* Questions:
	* Will you be including IE support?  Response being that can we record in Chrome and playback in other browsers?
	* Selenium will break based on changing tags.  How will this tool respond?  Response it is harder to work with pixels rather than the DOM - if it looks the same it is the same
	* How will this handle a large volume of tests?  How will you know status?  Response need to add reports.  Will have list a of results.  Need to speak afterwards to get an idea of the reports that might be useful
	* How trigger tests?  Response built API to execute via endpoint
	* How do you deal with animations?  Response only perform the visual match on click.  Waiting as long as the original person waiting on recording.
	* How does this compare to existing OCR software?  Response built own OCR as open source offering didn't support small fonts
	* Can you run this in parallel?  Response concurrency isn't a factor - its based on what you can afford in the cloud
	* Is there some thing smaller that you can take out of the system and offer?  Possibly components that others can use?  Response would be fairly easy to split out components if needs be
	* Any option to install on-premise?  Response always Docker containers... but hasn't been a priority to date.  financial services would want their data online
	* Will it be configurable so that elements can be changed without re-recording?  Response might be introduce complexity - but if that is what is needed, will look at adding some sort of data-driven elements