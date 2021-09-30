# Description
*This is a summarize of [The Agile Samurai Bootcamp](https://www.udemy.com/course/the-agile-samurai-bootcamp) course*

# Waterfall vs Agile

- Waterfall is essentially making a good plan and sticking to it.

- Agile utilises a more flexible, iterative approach.

# Agile
- **Not necessary for solo start-ups because you don't even have a working application yet.** [**The Lean Startup**](https://en.wikipedia.org/wiki/The_Lean_Startup)

<!-- - Suggested CI/CD program for Apple Ecosystem Development. [**Name Of Program**](./link) (Jira-complex? Trello-basic?) )  -->

### Kanban
- Do not prescribe roles like Scrum does, team structure can stay how it was.
- Changes can be made at any point in time, unlike Scrum has Sprints and changes decides according to customer feedback on this Sprints.
- Instead of *Velocity* and *Burndown Charts*, it has *Cycle Time* and *Lead Time*
  - **Cycle Time**: Measures how long it takes for a task to be completed.
  - **Lead Time**: Measures how long from when a task was added to your Kanban board until it was completed.
- Kanban is better for projects that you have done before(Recurring Similar Projects.) while Scrum is better for new challenging projects that are more deadline-oriented, and has many uncertainties.

### Scrum & XP(Extreme Programming)
- The way of thinking
  - Impossible to gather all the requirements at the start of the project.
  - Gathered requirements are guaranteed to change.
  - Requirements will always exceed time.

- Scrum is used for planning and XP for engineering.
- Term differences between Scrum and XP

	|      Scrum      |        XP         |
	| :-------------: | :---------------: |
	|     Sprint      |    Iterations     |
	| Product Backlog | Master Story List |
	|  Product Owner  |  Onsite Customer  |

---
## Team Creation
- Example Development Team
  - Agile Analyst: Creates Master Story Lists by bridging Development team and Customer. Helps Customer what he needs.
  - Agile Developer: Turns Master Story Lists into Software by coding & unit Testing.
  - Agile Tester: Writes tests for each story in the Lists before development process begins. (Exploratory, Stress Load, Security, Integration)
  - Agile Project Manager: Prepares Software Development Environment, tracks process(Time, Budged, Quality, Risk) of project and gives feedback to the team.

- Agile team must responsible from all work and kept informed about whole project in Sprits.
	<img src=".\Assets\agileTeam.png" alt="agileTeam" width="450" height="265" />

- If you create a new team to make team engaged, demo your software like you are presenting to the customer, see if its successfull then find bad parts and retry.

## Planning Process
- ### User Stories
	- Story Gathering Workshop: Get together customer and development team and write user stories, the goal is estimating total project date based on story list.
	- Do not write tech level explanation, explain with simple terms.
	- Do not write low level details.
	- Try smaller than one week(5 working days) stories to be completed until next Sprint.
	- If a story needs more time than a Sprint, it is called Epics (Big Stories).
	- Each story must be independent.
	- Each story must be testable.
	- Set testing criterias with customer, do not over test anything.

		<img src=".\Assets\testCriteria.png" alt="testCriteria" width="328" height="95" />

	- Set documenting criterias with customer, document as less as possible.
	- You have to persuade customer that stories may change according to project needs in the future.
	- Logically group stories from most important to less.
	- Limit your story count to 10-40 (3-6 months long) do not go beyond in the beginning, later you may make 1-3 months plans for future.
	- Story timing should be relative each other so that you can take reference and resize new stories according to the reference.

		<img src=".\Assets\sampleUserStories.png" alt="sampleUserStories" width="329" height="234" />

	- Multiply estimated points by reference date to calculate project time.
	- Use below template to create each story.

		<img src=".\Assets\exampleStory.png" alt="exampleStory" width="320" height="89" />

	- Make Poker Estimation for Story planning.

		<img src=".\Assets\pokerEstimation.png" alt="pokerEstimation" width="362" height="264" />

	- Complete Story List is called Master Story List.

- ### Delivery Options
	- Deliver by date.
	- Deliver by feature.

- ### Burndown chart
	Shows how fast our team burning down user stories.

  <img src=".\Assets\burnDownChart.png" alt="burnDownChart" width="732" height="439" />

  - When something unexpectedly occoured replan your burndown chart and calculate new estimated project delivery date.
  - [Burndown Chart Template](.\Assets\sampleBurnDownChart.xlsx)

- ### Strict project planning
	Create two Master Story List in the beginning of project, don't touch first one until the end of project, change second one according to project needs during project.

## Development Process
### Beginning Project
#### Master Story List Creation

### Beginning of Iteration(Sprint)
#### Customer Meetings

30-120 minutes meetings.

- Meet with customer for each iteration, try to force them to engage with your team even if they are unwilling to do that.
- Make sure previous iteration requirements is done before meeting for new iteration.
  - Only fully tested complete stories will be shown in iteration, if a story isn't fully completed, take it to the next iteration.
- Take feedback on completed iteration stories.
  - Have we done our homework?
  - Do you want additional tests?
- Plan next iteration stories with customer.
  - Are next iteration's stories good to go?
  - Do you want additional tests?
  - Tell customer the estimated time of planned iteration!
- Iteration 0 - Setup Phrase: Source control, development and test environments. (Xcode, Git, Fastlane setup etc...)

<img src=".\Assets\iterations.png" alt="iterations" width="735" height="294" />

#### Retrospective - Team Talks without Customer
15-30 minutes talks.

- Find out what are we doing well? Encourage good stuff say good things.
- Find out where can we do even better? Talk about it and share ideas.

### During Iteration(Sprint)
#### Daily stand-up
10-15 minutes talks.

- What did you do yesterday?
- What you will do today?
- What is your plan to solve existing problems?

### Development Rules
1. **Write tests before writing code!**
  1. Write all fail cases.
  2. Write all pass cases.
  3. Refactor code.
 
     > **Refactoring** is the practice of continuously making small, incremental design improvements to our software without changing overall external behavior. We aren't adding new fuctionality or fix bugs, instead we improve the understandability of code.

     <img src=".\Assets\writeTest.png" alt="writeTest" width="342" height="283" />

2. **Continuous Integration - Continuous Deployment (CI/CD)**

  Culture of production readiness, anyone, anytime, any where.

  <img src=".\Assets\pipeline.jpg" alt="pipeline" width="690" height="230" />

  1. CI/CD environment must be ready just before first iteration.
  2. CI/CD must be used for all iterations during project.
  3. Developers should pull existing code from Repository daily to their feature branch.
     <img src=".\Assets\cIMerging.png" alt="cIMerging" width="539" height="262" />
