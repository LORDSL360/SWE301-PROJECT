***
***4.1 Team Informantion***
-

***Project Title : Global Football Scouting & Analytics Platform***

***Group letter : F***


***Project members :***
1- Salman Yaqoub Yousef   , 2231153411 
2- Saad Khaled Saad       , 2231162401
3- Fahad Ahmad Almutairi  , 2231126794

***GitHub repository URL :*** https://github.com/LORDSL360/SWE301-PROJECT/


***One sentence project summary:***
A centralized scouting platform that enables clubs and scouts to easily discover and compare players worldwide through data driven insights



***4.2  Problems and Users***
-

Scouting football talent across different leagues today is still a messy and disconnected process. Clubs and independent scouts rely on a mix of scattered video clips, manual notes and spreadsheets to track players. Analysts spend hours jumping between different sources just to gather basic match stats and physical data. Because everyone uses different formats to rate players, reports end up being subjective and hard to compare. This slow and fragmented setup often causes communication delays, missed talent in lower divisions and bad transfer decisions that waste club budget
this issue affects three main groups:
.talent scouts: they need clean and structured way to write and submit match reports without dealing with multiple files and messy formats
.Technical Directors & Club Decision-Makers: They need clear, reliable data and insights to compare target players quickly and make confident transfer choices within their budget limit
.System administrators: they need full control over the platform to verify submitted data, manage user accounts and keep everything secure



***4.3 Existing Solutions***
-


***( 1 ) Current process:*** Manual spreadsheets & Messaging

• ***•  Useful features :*** low cost, familiar to traditional scouts and flexible free text notes.
• ***•  Limitation for your Users :*** Disjointed data, lack of visual comparisons, high risk of duplicate report, no standardized metric scaling
• ***•  Source :*** Field Interviews & Industry observation


***( 2 ) Existing Solution 1:*** Wyscout

• ***•  Useful features :*** Massive global video database, comprehensive player statistical coverage. 
• ***•  Limitation for your Users :*** High subscription cost for lower tier and regional clubs, complex interface and lacks customized internal club report workflows
• ***•  Source :*** https://wyscout.com/

***( 3 ) Existing Solution 2:*** BePro Football

***•  Useful features :*** High-quality tactical match video processing and automated event tracking.
***•  Limitation for your Users :*** focused primarily on team's own match analysis rather than global player scouting and cross league recruitment.
***•  Source :*** https://www.google.com/search?q=https://www.beproscore.com

After comparing these options, we noticed two main issues: existing platforms either way too expensive for smaller clubs or they focus heavily on match analysis instead of scouting new talent. Our platform fills this gap by combining easy to use scouting on match analysis forms with simple visual charts(like radar graphs) so club can quickly compare players and make practical recruitment choices without breaking their budget.


***4.4 Proposed Solution and Justification***
-

Our proposed solution is a centralized web platform built to make football recruitment simpler, faster, and more organized. The system allows Talent Scouts to fill out clean, standardized report forms, while Technical Directors & Club Decision-Makers can search, filter, and compare player stats using visual radar charts.

This system directly fixes the issues found in current processes and market tools:

***Improving the Current Process:*** Instead of relying on loose spreadsheets and scattered video links, our platform keeps everything in a single database. This makes player data searchable in seconds, uses a clear 1–10 rating scale, and keeps a clean history of all scouting reports.

***Fixing Market Limitations:*** High-end platforms like Wyscout are often too expensive and full of complex features that smaller clubs do not need. Our platform offers an affordable, easy-to-use alternative that focuses strictly on talent comparison and recruitment choices.

***Feasibility for a 3-Student Team:*** Building a massive live video platform in one semester is impossible for three students. To keep the workload realistic, our prototype will use structured mock datasets (PostgreSQL/JSON) and open-source chart components. This allows our team to focus entirely on perfecting the core workflows: entering scout reports, filtering players, and displaying side-by-side radar charts.

***Reused Libraries and Components:*** To speed up development and avoid recreating standard UI elements, we will use React and Tailwind CSS for the front-end, Chart.js (or Recharts) for rendering radar visual graphs, and Node.js with Express for building our backend APIs.




***4.5 Scope and Workflows***
-

***System Scope***

***1. In Scope (Semester Prototype)***

***What the semester prototype will include:***

•  Authentication and role-based access control (Scout, Analyst, Club Director, Admin).
• Standardized scout reporting form and review interface.
• Advanced search and filtering engine for emerging players.
• Interactive radar charts for side-by-side player comparison.
• Simulated database using PostgreSQL.


***2. Out of scope (future releases)***

• What the team will not attempt this semester:
• Live video upload, streaming, and AI video tracking.
• Integration with real-time paid commercial football data APIs.
• Financial contract management and direct club transfer negotiations.



  ***3. End-to-end Workflows:***

***Workflow 1:*** Search for an emerging player

***Main actor and goal:*** Talent Scout: Searches for a young emerging player (under 21) whose metrics indicate a "A rising talent" status.

***Expected outcome:*** A filtered list of promising players appears with brief summary statistics.


***Workflow 2:*** Submit a scout report

***Main actor and goal:*** Talent Scout: Fills out a standardized field evaluation form for a specific player after performance observation.

***Expected outcome:*** The report is saved to the database and linked to the player profile for decision-makers to view instantly.


***Workflow 3:*** Compare players and decide

***Main actor and goal:*** Club Director: Selects two emerging players to compare their attributes before recommending a transfer.

***Expected outcome:*** The system displays a side-by-side radar chart highlighting the strengths and weaknesses of each player.






***4.6 Initial Requirements***
-


#### Functional Requirements

| ID | Functional Requirement | Priority |
| :--- | :--- | :--- |
| **FR-01** | The system shall allow [المستخدم] to [الوظيفة أو السلوك المطلوب]. | **Must** |
| **FR-02** | The system shall allow [المستخدم] to [الوظيفة أو السلوك المطلوب]. | **Must** |
| **FR-03** | The system shall allow [المستخدم] to [الوظيفة أو السلوك المطلوب]. | **Must** |
| **FR-04** | The system shall allow [المستخدم] to [الوظيفة أو السلوك المطلوب]. | **Must** |
| **FR-05** | The system shall allow [المستخدم] to [الوظيفة أو السلوك المطلوب]. | **Must** |
| **FR-06** | The system shall allow [المستخدم] to [الوظيفة أو السلوك المطلوب]. | **Should** |
| **FR-07** | The system shall allow [المستخدم] to [الوظيفة أو السلوك المطلوب]. | **Should** |
| **FR-08** | The system shall allow [المستخدم] to [الوظيفة أو السلوك المطلوب]. | **Could** |

#### Non-Functional Requirements

| ID | Category | Measurable Requirement |
| :--- | :--- | :--- |
| **NFR-01** | **Performance** | The system shall [شرح المعيار المباشر والقابل للقياس، مثل زمن الاستجابة بالثواني]. |
| **NFR-02** | **Usability** | The system shall [شرح المعيار المباشر والقابل للقياس، مثل الوقت المستغرق لإتمام مهمة]. |
| **NFR-03** | **Security** | The system shall [شرح المعيار المباشر والقابل للقياس، مثل نوع التشفير أو التوثيق]. |




***4.7 Development Approach***
-
[شرح المنهجية المختارة في فقرة أو فقرتين - مثل Agile أو Hybrid].

How we use GitHub for collaboration:
[أكتب هنا طريقة العمل الجماعي على GitHub، مثل إنشاء الـ Branches، واستخدام الـ Pull Requests والـ Issues لتتبع المهام].




***4.8 Team Plan and Risks***
-


#### Team Coordinator Roles
* **Process and Project Coordinator:** [اسم الطالب] - [شرح مختصر للمسؤوليات وقيادة الـ GitHub Workflow].
* **Requirements and Design Coordinator:** [اسم الطالب] - [شرح مختصر لمسؤوليات المتطلبات وتصميم الواجهات].
* **Implementation and Quality Coordinator:** [اسم الطالب] - [شرح مختصر لمسؤوليات الكود واختبار جودة النظام].

#### Milestone Plan

| Milestone | Main Planned Output | Coordinator |
| :--- | :--- | :--- |
| **1. Proposal** | [المخرج الرئيسي للمرحلة الأولى] | Process & Project Coordinator |
| **2. Requirements & Models** | [المخرج الرئيسي للمرحلة الثانية] | Requirements & Design Coordinator |
| **3. Design & Initial Prototype** | [المخرج الرئيسي للمرحلة الثالثة] | Implementation & Quality Coordinator |
| **4. Final Prototype & Testing** | [المخرج الرئيسي للمرحلة الرابعة] | All Team Members |

#### Project Risks

| Risk | Impact | Planned Response |
| :--- | :--- | :--- |
| **[المخاطرة الأولى - مثل التعارض في كود GitHub]** | **High** | [الخطة المتبعة للتعامل مع الخطر] |
| **[المخاطرة الثانية - مثل تعقيد البيانات أو الميزانية]** | **Medium** | [الخطة المتبعة للتعامل مع الخطر] |
| **[المخاطرة الثالثة - مثل الأداء أو الواجهات]** | **Medium** | [الخطة المتبعة للتعامل مع الخطر] |




***4.9 Sources, AI Use, and Contributions***
-


#### Sources & References
1. [المصدر الأول - اسم المنصة أو الكتاب الرابط]
2. [المصدر الثاني - اسم المنصة أو الكتاب الرابط]
3. [المصدر الثالث - اسم المرجع الأكاديمي]

#### Generative AI Disclosure
* **Tool Used:** [اسم أداة الذكاء الاصطناعي]
* **How it was used:** [شرح كيف ساعدت الأداة في تحسين الصياغة أو تنظيم المستند]
* **Verification and Revision:** [شرح كيف قام الفريق بمراجعة وتعديل المخرجات والتأكد من صحتها]

#### GitHub Team Contributions


* **[اسم الطالب الأول]:** [توضيح المساهمات الفعلية والـ Commits التي قام بها في المستودع]
* **[اسم الطالب الثاني[توضيح المساهمات الفعلية والـ Commits التي قام بها في المستودع]
* **[اسم الطالب الثالث]:** [توضيح المساهمات الفعلية والـ Commits التي قام بها في المستودع]

***
