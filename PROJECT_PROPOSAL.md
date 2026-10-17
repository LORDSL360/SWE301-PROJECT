
***4.1 Team Informantion***
-

***Project Title : Global Football Scouting & Analytics Platform***

***Group letter : F***


***Project members :***
* ***1- Salman Yaqoub Yousef   , 2231153411***
* ***2- Saad Khaled Saad       , 2231162401***
* ***3- Fahad Ahmad Almutairi  , 2231126794***

***GitHub repository URL :*** https://github.com/LORDSL360/SWE301-PROJECT/


***One sentence project summary:***
A global scouting network which puts at the clubs and scouts’ fingertips the tool to find and compare players from around the world via data analytics.



***4.2  Problems and Users***
-

Scout report of football talent across various leagues is a very disjointed practice at present. Clubs and independent scouts use a mix of out of date video clips, pen and paper notes and spreadsheets to track players. Analysts spend time going back and forth between different sources just to get basic match stats and physical data. Due to the fact that everyone uses different systems to rate players reports come out subjective and hard to compare. This slow and fragmented system also causes delay in communication, we miss out on talent in lower divisions and we see bad transfer decisions which in turn waste club budget.

***this issue affects three main groups:***
-

* ***talent scouts:*** They require a simple and organized way to submit match reports which is free of multiple files and messy formats.
* ***Technical Directors & Club Decision-Makers:*** They require precise and trusted data which allows them to compare target players easily and within the budget to make sure their transfer choices are confident.
* ***System administrators:*** They require complete control over the platform to check in on submitted data, manage user accounts and keep it secure.



***4.3 Existing Solutions***
-


***( 1 ) Current process:*** Manual spreadsheets & Messaging

*  ***Useful features:*** low cost, familiar to traditional scouts and flexible free text notes.
*  ***Limitation for your Users:*** Disjointed data, lack of visual comparisons, high risk of duplicate report, no standardized metric scaling.
*  ***Source:*** Field Interviews & Industry observation.


***( 2 ) Existing Solution 1:*** Wyscout

 *   ***Useful features:*** Massive global video database, comprehensive player statistical coverage. 
 *   ***Limitation for your Users:*** High subscription cost for lower tier and regional clubs, complex interface and lacks customized internal club report workflows
 *   ***Source:*** https://wyscout.com/

***( 3 ) Existing Solution 2:*** BePro Football

*   ***Useful features:*** High-quality tactical match video processing and automated event tracking.
*   ***Limitation for your Users:*** focused primarily on team's own match analysis rather than global player scouting and cross league recruitment.
*   ***Source:*** https://www.google.com/search?q=https://www.beproscore.com

After comparing these options, we noticed two main issues: existing platforms either way too expensive for smaller clubs or they focus heavily on match analysis instead of scouting new talent. Our platform fills this gap by combining easy to use scouting on match analysis forms with simple visual charts(like radar graphs) so club can quickly compare players and make practical recruitment choices without breaking their budget.


***4.4 Proposed Solution and Justification***
-

Our put forth solution is a central web based platform which we have designed to improve and simplify football recruitment. We have created a system which which Talent Scouts use to fill out clean, standardized report forms and also Technical Directors and Club Decision Makers which they in turn use to search, filter and compare player stats via visual radar charts.

This system improves on present processes and markets tools:

***Improving the Current Process:*** Instead we have done away with the use of loose spreadsheets and separate video links which is what our platform does. We have put it all into one database. This which in turn makes player data search friendly in seconds, we use a 1 to 10 rating scale for clarity and also we have a clean history of all scouting reports.

***Fixing Market Limitations:*** High cost of which Wyscout and similar platforms may be out of reach for some and also are very feature rich in a way which smaller clubs do not require. Our platform is a more affordable and simple option that we put forward for talent comparison and recruitment.

***Feasibility for a 3-Student Team:*** In a short semester to build out a large scale live video platform with three of us is a no go. We went with structured mock datasets (PostgreSQL/JSON) and open source chart components for the prototype which in turn allows our team to put all our effort into the core features  putting together scout reports, player filtering, and out put of side by side radar charts.

***Reused Libraries and Components:*** To increase the pace of development and to avoid reinventing the wheel with standard UI elements we will use React and Tailwind CSS for the front end, Chart.js (or Recharts) for the rendering of radar visual graphs, and Node.js with Express for our backend APIs.




***4.5 Scope and Workflows***
-

***System Scope***

***1. In Scope (Semester Prototype)***

***What the semester prototype will include:***

 * Authentication and role-based access control (Scout, Analyst, Club Director, Admin).
 * Standardized scout report form and review interface.
 * Advanced search and filtering tools for new players.
 * Interactive radial charts for comparing players side by side.
 *  VSimulated database using PostgreSQL.


***2. Out of scope (future releases)***

***What the team will not attempt this semester:***

*  Live stream upload, streaming, and AI video tracking.
*  Integration with real time paid commercial football data.
*  Financial agreement administration and direct player transfers.



  ***3. End-to-end Workflows:***

***Workflow 1:*** Search for an emerging player
-
***Main actor and goal:*** Talent Scout: Searches for a young emerging player (under 21) whose metrics indicate a "A rising talent" status.

***Expected outcome:*** A listing of the best players that meets our filters along with brief stats.


***Workflow 2:*** Submit a scout report
-
***Main actor and goal:*** Talent Scout: Fills out a standardized field evaluation form for a specific player after performance observation.

***Expected outcome:*** The report goes into the database and is associated with the player profile for immediate access by decision makers.


***Workflow 3:*** Compare players and decide
-
***Main actor and goal:*** Club Director: Reports on two up and coming players in terms of their attributes which in turn will inform the recommendation for a transfer.

***Expected outcome:*** The system presents a comparison of each player’s strengths and weaknesses in a side by side radar chart.






***4.6 Initial Requirements***
-


#### Functional Requirements

| ID | Functional Requirement | Priority |
| :--- | :--- | :--- |
| **FR-01** | The system shall allow registered users to log in using their username , password]. | **Must** |
| **FR-02** | The system shall allow Talent Scouts to submit player evaluation reports using a standardized 1–10 rating scale]. | **Must** |
| **FR-03** | The system shall allow Talent Scouts to search and filter players by age, position, performance statistics]. | **Must** |
| **FR-04** |The system shall allow Club Directors to view player profiles , scouting reports]. | **Must** |
| **FR-05** | The system shall allow Club Directors to compare two players using radar charts]. | **Must** |
| **FR-06** | The system shall allow Talent Scouts to view their previously submitted scouting reports]. | **Should** |
| **FR-07** | The system shall allow Administrators to manage user accounts , roles]. | **Should** |
| **FR-08** | The system shall allow Club Directors to sort player search results by performance ratings]. | **Could** |

#### Non-Functional Requirements

| ID | Category | Measurable Requirement |
| :--- | :--- | :--- |
| **NFR-01** | **Performance** | The system shall display player search results within 3 seconds using the agreed demonstration dataset]. |
| **NFR-02** | **Usability** | The system shall allow at least 4 out of 5 test users to complete a scouting report within 5 minutes without assistance]. |
| **NFR-03** | **Security** | The system shall block unauthorized access to administrator functions in 100% of the defined access-control test cases]. |




***4.7 Development Approach***
-
Our team is going with the Incremental Development approach which we see as a way to roll out the Global Football Scouting  Analytics Platform in small manageable steps. Also we have it that some requirements may change as we get user feedback and this is what the incremental approach is for  to improve features without putting the whole system at risk. We will get input from what we present to groups of users like Talent Scouts and Club Directors after we release each increment.

In the first phase we will develop user authentication and player search using simulated data. In the second phase we will put in the standardized scouting reports and put away player evaluations. In the third phase we will develop player comparison which will use radar charts also we will test the main workflows. We will use React, Tailwind CSS, Chart.js, Node.js and Express to save development time. This approach we use allows our team of three students to manage the semester schedule, to reduce technical risks and to present a working prototype.

***4.8 Team Plan and Risks***
-

#### Team Coordinator Roles

 Process and Project Coordinator:
-
***Salman Yaqoub Yousef*** – Responsible for managing project progress, organizing team tasks, monitoring deadlines, and coordinating the GitHub workflow, including branches, pull requests, and merges.

 Requirements and Design Coordinator:
-
***Fahad Ahmad Almutairi*** – Responsible for organizing functional and non-functional requirements, coordinating system design, and planning user interfaces for player searching, scouting reports, and player comparison.

 Implementation and Quality Coordinator:
-
***Saad Khaled Saad*** – Responsible for coordinating system implementation, integrating the database and radar charts, testing system features, and ensuring software quality.

All team members will contribute to requirements, design, implementation, testing, and documentation.

#### Milestone Plan

| Milestone | Main Planned Output | Coordinator |
| :--- | :--- | :--- |
| **1. Proposal** | [Project proposal including the problem, proposed solution, and initial requirements.] | Process & Project Coordinator |
| **2. Requirements & Models** | [Detailed functional and non-functional requirements, use case diagrams, and system models.] | Requirements & Design Coordinator|
| **3. Design & Initial Prototype** | [Initial web prototype with user authentication, player search, and scouting report forms.] | Implementation & Quality |    | **4. Final Prototype & Testing** | [Completed prototype with radar chart comparisons, system testing, and final presentation.] | All Team Members |

#### Project Risks

* | Risk | Impact | Planned Response |
* | GitHub merge conflicts | High   | Use separate branches and review changes before merging. |
* | Incorrect player data  | Medium | Check player data and use a 1–10 rating scale.           |
* | Radar chart problems   | Medium | Test charts early and fix any errors.                    |


***4.9 Sources, AI Use, and Contributions***
-
#### Sources & References

* ***Wyscout:*** https://wyscout.com/
* ***BePro Football:*** https://www.bepro.ai/
* ***React:*** https://react.dev/
* ***Tailwind CSS:*** https://tailwindcss.com/
* ***Chart.js:*** https://www.chartjs.org/
* ***Node.js:*** https://nodejs.org/
* ***Express:*** https://expressjs.com/

***AI Use***

We used ChatGPT to help organize project ideas, write initial requirements, and improve our documentation. The team reviewed and revised the AI-generated content to ensure it matched our project requirements.

#### Generative AI Disclosure
* **Tool Used:** [ChatGPT (OpenAI)]
* **How it was used:** [To organize project ideas, improve writing, and help draft initial requirements.]
* **Verification and Revision:** [The team reviewed and edited the content to ensure it matched the project requirements.]

#### GitHub Team Contributions

* ***Salman Yaqoub Yousef:*** Project planning, problem description, and GitHub management.
* ***Saad Khaled Saad:*** Requirements analysis, system design, and documentation.
* ***Fahad Ahmad Almutairi:*** Functional and non-functional requirements, development planning, and project risks.

All team members will contribute to the project through GitHub commits and participate in development and testing.]
***
