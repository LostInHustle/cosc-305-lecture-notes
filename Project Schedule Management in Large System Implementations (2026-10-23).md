# Project Schedule Management in Large System Implementations

## Lecture Overview

This lecture examines project schedule management through the Integrated Renewal Program Student project at UBC. The project replaced UBC's legacy student information system with Workday Student and related supporting systems.

The central lesson is that project scheduling is not simply about selecting dates. It involves coordinating scope, people, technology, data, dependencies, risks, governance, and organizational change.

By the end of this lecture, you should be able to:

- Explain why large transformation projects are difficult to schedule
- Identify the major factors that influence a project schedule
- Compare common estimation techniques
- Describe how estimation changes as a project progresses
- Explain common schedule recovery strategies
- Recognize the importance of dependencies, communication, and stakeholder commitment

# 1. The Project Manager Scenario

Imagine that you are the project manager responsible for replacing a university student information system.

The system supports approximately 70,000 students and manages essential activities such as:

- Student applications
- Admissions
- Registration
- Academic records
- Program and course information
- Transfer credits
- Awards and student loans
- Tuition calculation
- Assessments and grades
- Academic progression
- Graduation

You are told that the existing system must be replaced within two or three years.

Your immediate concerns would probably include:

- How student data will be transferred
- How data accuracy will be maintained
- How personal information will be protected
- Whether the new system can handle thousands of simultaneous users
- Whether registration will remain available during busy periods
- How many people and departments will be affected
- Whether the project has enough funding and resources
- Whether staff, faculty, and students are prepared for the change
- What will happen if the project misses its required launch date

These concerns show why schedule management is not only about dates. A schedule must account for uncertainty, risk, organizational readiness, and coordination among many teams.

# 2. The IRP Student Context

UBC created the Integrated Renewal Program to modernize its human resources, finance, and student administration systems.

The first major implementation introduced Workday for human resources and finance in 2020.

The next major phase focused on replacing UBC's legacy student information system. Workday Student was implemented in 2024 as part of this transformation.

The project was expected to affect:

- Undergraduate students
- Graduate students
- Faculty members
- Staff members
- Academic advising offices
- Student service offices
- Administrative units
- Both UBC campuses
- Both university senates

This was not only a technology project. It was also a transformation involving:

- People
- Processes
- Data
- Governance
- Policy
- Communication
- Training
- Organizational change

Large transformation projects are especially challenging because all of these elements must work together.

# 3. The Scope of a Student Information System

A student information system manages the complete student lifecycle.

This lifecycle includes:

1. A student applies to the university.
2. The university reviews the application.
3. The student is admitted to a program.
4. The student accepts the offer.
5. The student registers for courses.
6. The university maintains the student's academic record.
7. The student receives grades and credits.
8. The university evaluates academic progression.
9. Tuition and fees are calculated.
10. Awards, loans, and financial support are managed.
11. The student completes program requirements.
12. The student graduates.

Each stage contains many rules, processes, data requirements, and system connections.

For example, registration must account for:

- Course availability
- Class capacity
- Prerequisites
- Program restrictions
- Year level
- Scheduling conflicts
- Waitlists
- Tuition implications
- Academic standing
- Registration time assignments

Registration is particularly risky because thousands of students may try to access the system at the same time. A performance problem could affect a large portion of the university.

## Key Principle

The complexity of a project schedule is directly related to the complexity of the project scope.

A larger or more complicated scope creates:

- More activities
- More dependencies
- More teams
- More decisions
- More testing
- More risks
- More opportunities for delay

Before creating a detailed schedule, the project manager must understand what the project is expected to deliver.

# 4. Program Teams and Shared Responsibility

The IRP Student program had more than 200 people working across several teams.

These teams included areas such as:

- Student solutions
- Change management
- Technical implementation
- Data conversion
- Quality assurance
- Testing
- Program management
- Business and stakeholder engagement

The student solutions team worked with university stakeholders to understand:

- Current business processes
- User requirements
- Existing problems
- Desired system capabilities
- Policy and operational needs

The data conversion team prepared legacy data for the new system.

The quality assurance and testing teams checked whether the system worked correctly.

The change management team helped staff, faculty, and students prepare for new processes and responsibilities.

The program management team coordinated scope, schedule, budget, risks, decisions, and communication.

## Who Owns the Schedule?

The project manager usually creates and maintains the schedule, but the project manager cannot deliver it alone.

Every team must:

- Provide realistic estimates
- Understand its commitments
- Complete assigned work
- Communicate risks early
- Coordinate with other teams
- Update progress honestly
- Support shared milestones

A schedule is only as reliable as the commitments behind it.

# 5. Factors That Influence a Project Schedule

Before estimating a project, the project manager must understand the conditions that will affect the work.

## 5.1 Project Scope

The project manager must understand:

- What functions are included
- What functions are excluded
- How complex the requirements are
- How many users will be affected
- How many business processes will change
- How many integrations are required
- How much data must be converted

A project replacing an entire student administration system will require more time than a project changing one registration feature.

## 5.2 Commercial Software or Custom Development

An organization must decide whether to:

- Purchase a commercial software product
- Build a custom system
- Use a combination of commercial and custom solutions

A commercial product may reduce the need to build a system from the beginning. However, the organization must understand:

- The maturity of the product
- The vendor's development roadmap
- Available product features
- Configuration limitations
- Required integrations
- The vendor's implementation experience

UBC selected Workday Student rather than building an entirely custom student system.

However, Workday Student could not meet every university need by itself. Supporting systems and integrations were still required. This increased the schedule complexity.

## 5.3 Organizational Size and Complexity

Important organizational factors include:

- Number of users
- Number of campuses
- Number of faculties and departments
- Number of programs
- Number of credentials
- Number of specializations
- Complexity of policies and processes
- Number of governance bodies

UBC operates across two campuses and has two senates. It also manages many programs, credentials, and specializations.

This creates additional requirements, approval processes, and dependencies.

## 5.4 Previous Experience

The organization should consider whether it has completed similar projects before.

Previous experience can provide:

- Historical estimates
- Lessons learned
- Reusable plans
- Experienced staff
- Known risks
- Better understanding of organizational capacity

A lack of experience may increase uncertainty.

## 5.5 Health of the Legacy System

If the existing system is unstable or approaching the end of its supported life, the project may face greater urgency.

However, urgency does not remove complexity. An aggressive schedule cannot make unclear requirements disappear.

## 5.6 Implementation Method

The project must decide how the work will be organized.

Common approaches include:

- Waterfall
- Agile
- A hybrid of waterfall and agile

The project must also decide whether implementation will be:

- Phased, where different components are introduced over time
- A single major launch, where many components are introduced together

IRP Student used a hybrid approach and organized major work into phases, work sets, and short sprints.

## 5.7 Timeline Constraints

Some deadlines cannot be moved easily.

For a university, the academic calendar creates important timing constraints.

For example, admissions for a future academic session may begin every September. If the system is not ready before the admissions cycle begins, the project may need to wait until the following annual cycle.

Missing one deadline could therefore create a delay of an entire year.

## 5.8 Budget Constraints

The project must operate within an approved budget.

Budget limits can affect:

- Team size
- External consulting support
- Testing capacity
- Training
- Technology choices
- Contingency
- Schedule recovery options

## 5.9 Regulation and Governance

The project may need to follow:

- Privacy requirements
- Security requirements
- Institutional policies
- Government regulations
- University governance processes
- Senate requirements
- Financial controls

Approvals and governance decisions must be included in the schedule.

## 5.10 Organizational Readiness for Change

People are the users of the new system.

The project must consider:

- Previous system implementations
- Staff workload
- Change fatigue
- Willingness to adopt new processes
- Training needs
- Communication needs
- Availability of subject experts

UBC staff and faculty had recently experienced the human resources and finance implementation. This created possible change fatigue that the student project needed to consider.

# 6. Estimation as the Foundation of Scheduling

A project schedule begins with estimates.

An estimate is a reasonable prediction of how much time or effort an activity may require.

Estimates are rarely exact because project teams do not have complete information at the beginning.

The goal of estimation is not to predict the future perfectly.

The goal is to make reasonable decisions using the best information currently available.

Estimates should become more detailed and dependable as the project progresses and more information becomes available.

# 7. Vacation Planning Example

Suppose someone asks:

How long will it take to plan a vacation to Europe?

You might initially answer:

- One week
- One month
- Two months

However, before providing a reliable answer, you would need more information.

You might ask:

- Which countries will be visited?
- How many people are travelling?
- How long is the vacation?
- What is the budget?
- Are visas required?
- Have passports been obtained?
- How will transportation be arranged?
- Where will the travellers stay?
- What activities are planned?
- Are there health or insurance requirements?

The same principle applies to project estimation.

A project manager begins by asking questions, identifying activities, and understanding constraints.

# 8. Common Estimation Techniques

## 8.1 Top Down Estimation

Top down estimation begins with the project as a whole.

The estimate is based on general experience, broad assumptions, or knowledge of similar types of work.

### Example

Most projects of this type take approximately three years, so this project may also take about three years.

For vacation planning:

Most people need about one month to prepare for this type of trip, so I will also estimate one month.

### Advantages

- Fast
- Simple
- Useful during early planning
- Does not require detailed activity information
- Helps leaders make initial funding decisions

### Limitations

- Less detailed
- Less precise
- May overlook important activities
- Depends heavily on assumptions
- Can create unrealistic expectations if treated as a final estimate

Top down estimates are most useful when the project is still being defined.

## 8.2 Analogous Estimation

Analogous estimation uses information from a similar past project.

### Example

A similar university completed a student system implementation in three years. Based on differences in size and complexity, this project may take three and a half years.

For vacation planning:

A similar trip took six weeks to prepare last year, so this trip may also require about six weeks.

### Advantages

- Uses real project experience
- Faster than detailed estimation
- Useful when historical information exists
- Can provide a reasonable early estimate

### Limitations

- No two projects are identical
- Historical data may be incomplete
- Differences in scope may be overlooked
- Changes in technology or staffing may reduce comparability

The project manager must adjust the estimate for differences in scope, complexity, resources, and risk.

## 8.3 Bottom Up Estimation

Bottom up estimation divides the project into smaller activities.

Each activity is estimated separately. The individual estimates are then combined.

### Example

A system implementation might include:

- Requirements analysis
- System design
- Configuration
- Data conversion
- Integration development
- Testing
- Training
- Deployment

If requirements take six weeks, design takes eight weeks, and testing takes twelve weeks, these estimates can be combined with the remaining activities to build the overall schedule.

For vacation planning, separate estimates could be created for:

- Finding flights
- Booking hotels
- Applying for visas
- Planning transportation
- Selecting activities
- Purchasing insurance
- Preparing travel documents

### Advantages

- More detailed
- Usually more accurate
- Makes assumptions visible
- Helps identify dependencies
- Supports resource planning

### Limitations

- Requires more time
- Requires more information
- May not be practical during early planning
- Can still be inaccurate if activities are missing

Bottom up estimation becomes more useful after the project scope is better understood.

## 8.4 Expert Judgement

Expert judgement uses the knowledge of experienced people.

Experts may include:

- Project managers
- Technical leads
- Data specialists
- Testing leads
- Business analysts
- Change management specialists
- Vendor representatives
- People who completed similar projects

### Example

A testing lead reviews the number of business processes, integrations, and user groups. The testing lead then estimates that testing will require four months.

### Advantages

- Practical
- Based on experience
- Useful when historical data is limited
- Can identify risks that others may miss

### Limitations

- May be influenced by personal bias
- Different experts may provide different estimates
- Experts may be overly optimistic or overly cautious
- Estimates should still be validated

Expert judgement is most reliable when several knowledgeable people review the estimate and explain their assumptions.

## 8.5 Three Point Estimation

Three point estimation considers three possible scenarios.

### Optimistic Estimate

The time required if everything goes well.

### Most Likely Estimate

The expected time based on normal conditions.

### Pessimistic Estimate

The time required if significant problems occur.

### Example

For an activity:

- Optimistic estimate: two weeks
- Most likely estimate: four weeks
- Pessimistic estimate: eight weeks

A simple average would be:

Two plus four plus eight equals fourteen.

Fourteen divided by three equals approximately 4.7 weeks.

A weighted approach can place more emphasis on the most likely estimate:

Expected time equals optimistic plus four times most likely plus pessimistic, all divided by six.

Using the example:

Expected time equals two plus sixteen plus eight, all divided by six.

Expected time equals approximately 4.3 weeks.

### Advantages

- Recognizes uncertainty
- Encourages discussion of risk
- Provides a range of possible outcomes
- Reduces dependence on one estimate

### Limitations

- Requires additional analysis
- Depends on realistic scenarios
- Can still be biased
- Takes more time than a single estimate

# 9. Combining Estimation Techniques

There is no single best estimation method for every situation.

Strong projects often combine several methods.

For example:

1. Use top down estimation to create an initial project range.
2. Review similar projects using analogous estimation.
3. Ask experienced leaders for expert judgement.
4. Develop bottom up estimates as requirements become clearer.
5. Apply three point estimation to uncertain or risky activities.

Combining methods provides a stronger estimate than relying on only one method.

# 10. Estimation Changes Over Time

At the beginning of a project:

- Information is limited
- Scope may be unclear
- Detailed planning may not be possible
- Estimates have greater uncertainty

During this stage, the project may use:

- Top down estimation
- Analogous estimation
- Expert judgement

As the project progresses:

- Requirements become clearer
- Activities can be divided into smaller pieces
- Dependencies become visible
- Team members understand the work better
- Estimates can be refined

Later stages may use:

- Bottom up estimation
- Three point estimation
- Detailed expert judgement
- Team based sprint planning

This process is sometimes described as progressive elaboration. The project plan becomes more detailed as knowledge increases.

The schedule should not remain unchanged simply because an early estimate was approved. It should be refined when better information becomes available.

# 11. The IRP Student Planning Structure

The project used a hybrid planning structure.

At a high level, major phases included activities such as:

- Planning
- Architecture
- Prototyping
- Design
- Configuration
- Testing
- Deployment

Some phases lasted several years. It was not practical to plan every detail for the entire period at the beginning.

The project therefore divided major phases into smaller work sets.

Each work set had a defined scope and specific outcomes.

Examples of work set content could include:

- Admissions
- Academic records
- Registration
- Program management
- Student finance
- Graduation

The work sets were further divided into approximately two week sprints.

For each sprint, teams determined:

- What work would be completed
- Who would perform the work
- What dependencies existed
- Whether the work could be completed within one sprint
- What risks might prevent completion
- What decisions or approvals were required

This structure allowed the project to maintain a long term direction while planning near term work in greater detail.

# 12. What Happens When a Project Falls Behind?

Imagine that the project is six months away from launch and is behind schedule.

The launch date cannot move because missing it would interfere with the university's annual academic cycle.

The project must consider schedule recovery strategies.

Each strategy creates tradeoffs. There is no free way to compress a schedule.

# 13. Schedule Recovery Strategies

## 13.1 Fast Tracking

Fast tracking means performing activities in parallel that were originally planned in sequence.

### Example

Instead of waiting for all design work to finish before testing begins, the project might begin testing completed parts while design continues elsewhere.

### Benefit

The project may save time by overlapping activities.

### Risks

- Rework may be required
- Incomplete information may cause errors
- Teams may become overloaded
- Coordination becomes more difficult
- Quality may decline

Fast tracking is only possible when dependencies allow activities to overlap.

## 13.2 Crashing

Crashing means adding resources to critical activities to reduce their duration.

The project might:

- Hire temporary staff
- Use external consultants
- Reassign people from less urgent work
- Add testing capacity
- Increase technical support
- Approve additional paid work hours where appropriate

### Benefit

Additional capacity may help complete critical work faster.

### Risks

- Costs increase
- New staff require orientation
- Additional people may create communication overhead
- Some work cannot be divided among more people
- Existing experts may spend time training new team members

Adding more people does not automatically make every activity faster.

## 13.3 Scope Reduction

The project may review the scope and focus on the minimum viable product.

The minimum viable product contains the smallest set of functions required for a usable and acceptable launch.

### Possible Actions

- Delay lower priority features
- Simplify a process
- Move optional reports to a later release
- Reduce customization
- Postpone nonessential integrations

### Risks

- Users may receive fewer capabilities
- Deferred work must still be completed later
- Business processes may require temporary solutions
- Stakeholders may disagree about what is essential

Scope changes require consultation and approval from business owners, sponsors, and governance bodies.

## 13.4 Phased Implementation

The project may introduce some functions at launch and others later.

### Benefit

A smaller initial launch may reduce immediate workload and risk.

### Risks

- Temporary connections may be required
- Users may need to work across old and new systems
- Data may need to be synchronized
- The overall transformation may take longer

## 13.5 Quality or Requirement Adjustment

The project may reconsider how some requirements are handled during the first release.

This does not mean ignoring essential quality, security, privacy, or legal requirements.

Instead, the project may determine whether a lower priority requirement can be addressed differently or completed later.

Any adjustment must be reviewed carefully and approved by the appropriate stakeholders.

# 14. Data Conversion Example

Legacy systems often contain inconsistent data.

For example, a province could appear as:

- British Columbia
- BC
- B C

Postal codes might contain:

- Missing spaces
- Incorrect characters
- Incomplete values
- Different formats

The new system may require one consistent format.

The project must decide whether to:

- Clean every legacy record before launch
- Convert only essential records
- Leave some optional fields blank
- Ask users to update information in the new system
- Complete some data improvements after launch

Correcting every record before launch could require months of work.

The project may instead decide to transfer essential information first and allow students or staff to update less critical data later.

This is a schedule decision, but it also affects:

- Data quality
- User experience
- Operational workload
- Privacy
- Reporting
- Stakeholder trust

Therefore, the decision must involve business owners, data experts, technical teams, and governance leaders.

# 15. Major Lessons Learned

## 15.1 The Critical Path Can Change

The critical path is the sequence of activities that determines the earliest possible project completion date.

Project managers may identify an initial critical path, but it can change when:

- New risks appear
- An activity takes longer than expected
- A dependency changes
- A required decision is delayed
- New work is discovered
- Resources become unavailable

The critical path must be monitored throughout the project, not only during initial planning.

## 15.2 Schedule Risk Often Exists Between Teams

Many delays are not caused by an individual failing to complete assigned work.

Delays often occur when one team is waiting for:

- Another team's deliverable
- A technical decision
- A business approval
- Data from another group
- An integration
- A policy interpretation
- A governance decision

The handoff between teams is often more dangerous than the work within one team.

Project managers must actively monitor dependencies and handoffs.

## 15.3 An Aggressive Schedule Cannot Fix Unclear Scope

A short timeline does not make complex requirements easier to understand.

If scope is unclear, teams may:

- Build the wrong solution
- Repeat work
- Discover missing requirements late
- Create unrealistic estimates
- Miss important dependencies
- Increase testing problems

Time spent clarifying scope early often saves time later.

## 15.4 Schedule Recovery Always Has a Cost

When a project falls behind, recovery options exist, but every option creates a tradeoff.

For example:

- Adding resources increases cost
- Fast tracking increases risk and possible rework
- Reducing scope decreases initial functionality
- Phased implementation increases transition complexity
- Reducing contingency leaves less protection against future problems

There is no free schedule compression.

## 15.5 A Schedule Must Be Believed

A highly detailed schedule is not useful if team members do not understand or support it.

An effective schedule is one that people:

- Understand
- Trust
- Update regularly
- Use to make decisions
- Connect to their own work
- Accept responsibility for delivering

A simple and realistic schedule is often more valuable than a complicated schedule that nobody follows.

# 16. Communication as the Foundation of Schedule Management

Schedule management is ultimately about communication.

A schedule must communicate:

- What needs to be completed
- Who is responsible
- When work is expected
- What dependencies exist
- What decisions are needed
- What risks are emerging
- What has changed
- What support is required

Project management software can store dates and activities, but software cannot create commitment.

A schedule succeeds when teams communicate honestly, understand the plan, and coordinate their work.

# 17. Applying These Techniques Across Industries

Project scheduling techniques can be used in many industries, including:

- Information technology
- Construction
- Health care
- Education
- Government
- Finance
- Engineering

The techniques may remain similar:

- Top down estimation
- Analogous estimation
- Bottom up estimation
- Expert judgement
- Three point estimation
- Fast tracking
- Crashing
- Scope review

However, the project context changes.

A construction project may need to consider:

- Permits
- Weather
- Materials
- Site conditions
- Building inspections
- Contractor availability

A health care project may need to consider:

- Patient safety
- Clinical workflows
- Medical regulations
- Privacy
- Staff training
- Service continuity

A technology project may need to consider:

- System performance
- Cybersecurity
- Data conversion
- Integrations
- Testing
- Vendor readiness

The project manager must understand the specific domain, identify the right experts, and apply scheduling techniques within that context.

# 18. Final Takeaways

The most important lessons from this lecture are:

1. Scheduling is more than selecting dates.

2. Scope complexity directly affects schedule complexity.

3. Early estimates are uncertain because information is incomplete.

4. Different estimation methods are appropriate at different stages.

5. Strong projects combine multiple estimation techniques.

6. Estimates should be refined as more information becomes available.

7. Dependencies between teams are a major source of schedule risk.

8. The critical path can change throughout the project.

9. Schedule recovery strategies always involve tradeoffs.

10. An aggressive timeline cannot replace clear requirements.

11. A schedule is only reliable when teams understand and support it.

12. Communication is one of the most important project management skills.

# Core Message

Good schedule management is not the ability to create a perfect plan at the beginning.

Good schedule management is the ability to create a reasonable plan, communicate it clearly, monitor it continuously, and adapt it responsibly as the project changes.
