# Lecture Notes: Project Scheduling, CPM, and PERT

## Learning Objectives

By the end of this lecture, you should be able to:

1. Explain where scheduling fits within project management.
2. Describe how a Work Breakdown Structure supports schedule development.
3. Define project activities and identify their dependencies.
4. Distinguish among the four main activity relationships.
5. Explain lead time, lag time, and milestones.
6. Compare Gantt charts with project network diagrams.
7. Perform a forward pass and a backward pass.
8. Calculate earliest start, earliest finish, latest start, latest finish, and slack.
9. Identify the critical path.
10. Explain the difference between CPM and PERT.
11. Calculate PERT expected time, variance, and standard deviation.
12. Use a Z score to estimate the probability of meeting a project deadline.
13. Explain the basic idea behind project crashing.

---

# 1. Course Reminders

Based on the lecture recording:

- Friday's class will be online.
- Students do not need to come to the classroom on Friday.
- Friday's session may involve a guest speaker.
- Check the course platform for the exact time and access information.
- Complete the required survey or registration form.
- The survey may be required to receive access to the Smartsheet activity.
- Review the scheduling material before the next class.
- The next class will include additional practice and examples.

Some timing details in the recording were unclear, so the course platform should be treated as the official source for deadlines and session times.

---

# 2. Where Scheduling Fits in Project Management

A project normally moves through several major phases:

1. Initiation
2. Planning
3. Execution
4. Monitoring and control
5. Closing

## 2.1 Initiation Phase

The initiation phase formally begins the project.

A major output of this phase is the project charter.

The project charter may include:

- Project purpose
- Project objectives
- High-level scope
- Initial budget
- Major stakeholders
- Project manager
- Sponsor or client commitment
- Major assumptions
- Major constraints

Once the project charter is approved, the project can move into detailed planning.

## 2.2 Planning Phase

The planning phase identifies how the project will be completed.

Planning may include:

- Scope planning
- Schedule planning
- Cost planning
- Resource planning
- Risk planning
- Quality planning
- Communication planning
- Procurement planning
- Stakeholder planning

Planning often requires a large amount of the project manager's time.

Good planning reduces confusion during project execution.

---

# 3. From Scope Planning to Schedule Planning

Before a schedule can be developed, the project manager must understand the work that needs to be completed.

One of the main outputs of scope planning is the Work Breakdown Structure.

## 3.1 Work Breakdown Structure

A Work Breakdown Structure is usually abbreviated as WBS.

A WBS divides the total project into smaller and more manageable pieces of work.

The WBS answers the following question:

> What work must be completed to deliver the project?

A WBS does not normally show:

- The sequence of activities
- The duration of activities
- The exact start and finish dates
- The relationships between activities
- The critical path
- The overall project completion time

Those details are developed during project scheduling.

## 3.2 Work Packages

The lowest useful level of a WBS is normally called a work package.

A work package is a manageable unit of project work.

A work package should be detailed enough that the project team can:

- Estimate its cost
- Estimate its duration
- Assign responsibility
- Monitor its progress

One work package may become one activity or several activities in the project schedule.

---

# 4. WBS Example: Wedding Project

Suppose the project is to organize a wedding.

The major areas of work may include:

- Invitations
- Food
- Ceremony
- Venue
- Guest management
- Entertainment

The invitation section may be divided into:

1. Create the guest list.
2. Design the invitations.
3. Print the invitations.
4. Address the envelopes.
5. Mail the invitations.
6. Collect guest responses.

The food section may be divided into:

1. Select a menu.
2. Identify dietary requirements.
3. Choose a caterer.
4. Confirm the number of guests.
5. Arrange food delivery.
6. Serve the food.

The WBS identifies the required work.

The schedule identifies when and in what order that work should be completed.

---

# 5. Main Steps in Project Scheduling

A simplified schedule development process is:

1. Define activities.
2. Sequence activities.
3. Estimate activity resources.
4. Estimate activity durations.
5. Develop the project schedule.
6. Identify milestones.
7. Identify the critical path.
8. Monitor and update the schedule.

The lecture focused mainly on the following process:

    WBS
    -> Activity list
    -> Activity sequence
    -> Duration estimates
    -> Network diagram
    -> Forward pass
    -> Backward pass
    -> Slack calculation
    -> Critical path
    -> Final project schedule

---

# 6. Defining Project Activities

Activities are developed from the work packages in the WBS.

A simple work package may become one activity.

A complex work package may need to be divided into several activities.

## Example

Suppose the WBS contains the work package:

    Prepare invitations

This work package may be divided into the following activities:

1. Create the guest list.
2. Design the invitation.
3. Approve the design.
4. Print the invitations.
5. Address the envelopes.
6. Mail the invitations.
7. Record responses.

The output of this process is an activity list.

A good activity should be specific enough that the team can estimate its duration and determine its relationships with other activities.

---

# 7. Sequencing Activities

After the activities have been identified, the next step is to place them in a logical sequence.

Some activities must be completed before other activities can begin.

For example:

- Food must be cooked before it can be served.
- Requirements should be collected before development begins.
- Invitations must be printed before they can be mailed.
- A venue should be booked before final setup planning is completed.

## 7.1 Predecessor

A predecessor is an activity that comes before another activity.

## 7.2 Successor

A successor is an activity that follows another activity.

## Example

If Activity A must be completed before Activity B can begin:

- Activity A is the predecessor.
- Activity B is the successor.

The relationship can be represented as:

    Activity A -> Activity B

---

# 8. Four Types of Activity Relationships

There are four main ways activities can be logically related.

These relationships are:

1. Finish to Start
2. Start to Start
3. Finish to Finish
4. Start to Finish

---

## 8.1 Finish to Start

Finish to Start is abbreviated as FS.

In a Finish to Start relationship, the predecessor must finish before the successor can start.

This is the most common type of relationship.

### Example

- Activity A: Cook the food
- Activity B: Serve the food

The food must be cooked before it can be served.

    Cook the food -> Serve the food

Another example is:

- Activity A: Print invitations
- Activity B: Mail invitations

The invitations must be printed before they can be mailed.

---

## 8.2 Start to Start

Start to Start is abbreviated as SS.

In a Start to Start relationship, the successor cannot start until the predecessor has started.

The two activities do not necessarily have to start at exactly the same moment.

The relationship means that the first activity must begin before the second activity is allowed to begin.

### Example

Suppose two people are cleaning a classroom:

- One person begins moving the chairs.
- Another person begins moving the tables.

The activities can occur at approximately the same time.

    Start moving chairs -> Start moving tables

The work can overlap because both activities help create space in the room.

---

## 8.3 Finish to Finish

Finish to Finish is abbreviated as FF.

In a Finish to Finish relationship, the successor cannot finish until the predecessor has finished.

The activities may begin at different times, but their completion is connected.

### Example

Suppose breakfast includes toast and eggs.

The activities may be scheduled so that the toast and eggs finish at approximately the same time.

This prevents one item from becoming cold while waiting for the other item.

---

## 8.4 Start to Finish

Start to Finish is abbreviated as SF.

In a Start to Finish relationship, the successor cannot finish until the predecessor has started.

This type of relationship is less common.

### Example

A delivery driver is unloading materials.

The driver cannot finish the delivery process and leave until the receiving employee begins the inspection or acceptance process.

The start of the receiving activity allows the delivery activity to finish.

---

# 9. Types of Dependencies

Dependencies may also be classified according to why they exist.

## 9.1 Mandatory Dependency

A mandatory dependency is required by the nature of the work.

Examples:

- Concrete must be poured before it can dry.
- Software must be developed before it can be tested.
- Food must be cooked before it can be served.

Mandatory dependencies are sometimes called hard logic.

## 9.2 Discretionary Dependency

A discretionary dependency is based on a preferred method, organizational practice, or team decision.

Examples:

- The team prefers to finish the complete design before development begins.
- Management prefers to approve every document before the next document is created.

The relationship may be useful, but it is not always technically required.

Discretionary dependencies are sometimes called soft logic.

## 9.3 External Dependency

An external dependency involves something outside the direct control of the project team.

Examples:

- Government approval
- Vendor delivery
- Client sign-off
- Equipment arrival
- Weather conditions
- Regulatory inspection

External dependencies can create schedule risk because the project manager may have limited control over them.

## 9.4 Internal Dependency

An internal dependency exists between activities that are under the control of the project team.

Example:

- The development team must finish coding before the internal testing team starts testing.

---

# 10. Lead Time and Lag Time

Lead and lag are used to adjust the timing between related activities.

## 10.1 Lag Time

Lag time is a required waiting period between two activities.

### Example

After painting a wall, the team must wait two days before applying another coating.

    Paint the wall
    -> Wait 2 days
    -> Apply the next coating

The two-day waiting period is the lag.

Another example is waiting for concrete to cure before construction continues.

## 10.2 Lead Time

Lead time allows a successor activity to begin before its predecessor is completely finished.

Lead time creates an overlap between activities.

### Example

Testing may begin on completed software modules before development of the entire application is finished.

If testing begins two days before development is fully complete, the relationship contains two days of lead time.

Lead time may shorten the project schedule, but it can also increase coordination risk.

---

# 11. Milestones

A milestone is an important checkpoint or event in a project.

A milestone usually represents:

- Completion of a major deliverable
- Completion of a major group of activities
- Approval of an important document
- Completion of a project phase
- A major client decision
- An important deadline

Milestones normally have zero duration.

A milestone records that something important has happened, but it does not represent work that continues for several days or weeks.

## Examples of Milestones

- Project charter approved
- Requirements document completed
- Invitations sent
- Menu finalized
- Venue booked
- Development completed
- Testing approved
- Final report submitted
- Product launched

Milestones help the project manager determine whether the project is progressing according to plan.

---

# 12. Gantt Charts

A Gantt chart displays project activities as horizontal bars across a timeline.

The left side normally lists the project activities.

The horizontal axis represents time, such as:

- Days
- Weeks
- Months
- Quarters

Each bar shows when an activity starts and finishes.

A Gantt chart may also show:

- Activity duration
- Milestones
- Dependencies
- Assigned resources
- Percentage complete
- Planned dates
- Actual dates
- Critical activities

## 12.1 Advantages of Gantt Charts

Gantt charts are:

- Easy to understand
- Useful for communication
- Useful for assigning work
- Useful for showing activity duration
- Useful for showing overlapping activities
- Useful for tracking progress
- Useful for presenting schedules to stakeholders

## 12.2 Limitations of Gantt Charts

Gantt charts can become difficult to read when:

- The project contains many activities.
- The project contains many dependencies.
- The chart is not updated regularly.
- The chart contains too much information.

Complex network logic may be easier to analyze using a project network diagram.

## 12.3 Main Purpose

A Gantt chart is especially useful for communicating the project schedule.

---

# 13. Project Network Diagrams

A project network diagram shows activities and the logical relationships among them.

In an Activity on Node network:

- Each node represents an activity.
- Each arrow represents a dependency.
- Activities flow from project start to project finish.

A detailed node may contain:

- Activity name
- Activity duration
- Earliest start
- Earliest finish
- Latest start
- Latest finish
- Slack

Network diagrams are useful for:

- Understanding activity sequence
- Performing CPM calculations
- Identifying the critical path
- Calculating schedule flexibility
- Analyzing the effect of delays

---

# 14. Important Scheduling Terms

## 14.1 Activity Duration

Activity duration is the amount of working time required to complete an activity.

Duration may be measured in:

- Hours
- Days
- Weeks
- Months

## 14.2 Earliest Start

Earliest Start is abbreviated as ES.

ES is the earliest time an activity can begin after considering its predecessors.

## 14.3 Earliest Finish

Earliest Finish is abbreviated as EF.

EF is the earliest time an activity can finish.

The formula is:

    EF = ES + Duration

## 14.4 Latest Finish

Latest Finish is abbreviated as LF.

LF is the latest time an activity can finish without delaying the planned project completion time.

## 14.5 Latest Start

Latest Start is abbreviated as LS.

LS is the latest time an activity can start without delaying the planned project completion time.

The formula is:

    LS = LF - Duration

## 14.6 Slack

Slack is the amount of time an activity can be delayed without delaying the planned project completion time.

Slack is also called float.

The formulas are:

    Slack = LS - ES

or:

    Slack = LF - EF

Both formulas should produce the same result.

## 14.7 Critical Activity

A critical activity is an activity with zero slack.

If a critical activity is delayed, the whole project will normally be delayed unless corrective action is taken.

---

# 15. Critical Path Method

Critical Path Method is abbreviated as CPM.

CPM is used to determine:

- The earliest possible project completion time
- The earliest start and finish time for each activity
- The latest start and finish time for each activity
- The slack for each activity
- The critical activities
- The critical path

Traditional CPM uses one estimated duration for each activity.

This means the activity durations are treated as deterministic.

## Main CPM Steps

1. List the activities.
2. Record the duration of each activity.
3. Identify the immediate predecessor of each activity.
4. Draw the project network.
5. Perform the forward pass.
6. Determine the minimum project completion time.
7. Perform the backward pass.
8. Calculate slack.
9. Identify the critical activities.
10. State the critical path.

---

# 16. CPM Example

Consider the following project.

| Activity | Duration | Immediate Predecessor |
| :------- | -------: | :-------------------- |
| A        |  7 weeks | None                  |
| B        |  9 weeks | None                  |
| C        | 12 weeks | A                     |
| D        |  8 weeks | A and B               |
| E        |  9 weeks | D                     |
| F        |  6 weeks | C and E               |
| G        |  5 weeks | E                     |

Activities A and B have no predecessors.

Therefore, A and B can begin at the start of the project.

The network contains the following relationships:

    Start -> A
    Start -> B
    A -> C
    A -> D
    B -> D
    D -> E
    C -> F
    E -> F
    E -> G
    F -> Finish
    G -> Finish

---

# 17. Forward Pass

The forward pass calculates ES and EF.

The calculation begins at the start of the network and moves toward the finish.

## 17.1 Forward Pass Rules

For an activity with no predecessor:

    ES = 0

For any activity:

    EF = ES + Duration

If an activity has more than one predecessor:

    ES = Maximum EF of all immediate predecessors

The maximum is used because every required predecessor must be complete before the activity can begin.

## Memory Rule

> Forward pass means add and take the maximum.

---

## 17.2 Activity A

Activity A has no predecessor.

    ES of A = 0
    EF of A = 0 + 7
    EF of A = 7

Therefore:

| Activity |  ES |  EF |
| :------- | --: | --: |
| A        |   0 |   7 |

---

## 17.3 Activity B

Activity B has no predecessor.

    ES of B = 0
    EF of B = 0 + 9
    EF of B = 9

Therefore:

| Activity |  ES |  EF |
| :------- | --: | --: |
| B        |   0 |   9 |

---

## 17.4 Activity C

Activity C depends on Activity A.

Activity A finishes at week 7.

    ES of C = EF of A
    ES of C = 7

Activity C has a duration of 12 weeks.

    EF of C = 7 + 12
    EF of C = 19

Therefore:

| Activity |  ES |  EF |
| :------- | --: | --: |
| C        |   7 |  19 |

---

## 17.5 Activity D

Activity D depends on both A and B.

The predecessor finish times are:

    EF of A = 7
    EF of B = 9

Activity D cannot begin until both A and B are complete.

Therefore, use the larger value.

    ES of D = Maximum of 7 and 9
    ES of D = 9

Activity D has a duration of 8 weeks.

    EF of D = 9 + 8
    EF of D = 17

Therefore:

| Activity |  ES |  EF |
| :------- | --: | --: |
| D        |   9 |  17 |

---

## 17.6 Activity E

Activity E depends on D.

    ES of E = EF of D
    ES of E = 17

Activity E has a duration of 9 weeks.

    EF of E = 17 + 9
    EF of E = 26

Therefore:

| Activity |  ES |  EF |
| :------- | --: | --: |
| E        |  17 |  26 |

---

## 17.7 Activity F

Activity F depends on C and E.

The predecessor finish times are:

    EF of C = 19
    EF of E = 26

Activity F must wait until both predecessors are complete.

Therefore, use the larger value.

    ES of F = Maximum of 19 and 26
    ES of F = 26

Activity F has a duration of 6 weeks.

    EF of F = 26 + 6
    EF of F = 32

Therefore:

| Activity |  ES |  EF |
| :------- | --: | --: |
| F        |  26 |  32 |

---

## 17.8 Activity G

Activity G depends on E.

    ES of G = EF of E
    ES of G = 26

Activity G has a duration of 5 weeks.

    EF of G = 26 + 5
    EF of G = 31

Therefore:

| Activity |  ES |  EF |
| :------- | --: | --: |
| G        |  26 |  31 |

---

# 18. Minimum Project Completion Time

The project has two ending activities:

- Activity F
- Activity G

Their earliest finish times are:

    EF of F = 32
    EF of G = 31

The project is not complete until all required ending activities are complete.

Therefore:

    Minimum project completion time
    = Maximum of 32 and 31
    = 32 weeks

The earliest possible project completion time is 32 weeks.

---

# 19. Forward Pass Results

| Activity | Duration |  ES |  EF |
| :------- | -------: | --: | --: |
| A        |        7 |   0 |   7 |
| B        |        9 |   0 |   9 |
| C        |       12 |   7 |  19 |
| D        |        8 |   9 |  17 |
| E        |        9 |  17 |  26 |
| F        |        6 |  26 |  32 |
| G        |        5 |  26 |  31 |

---

# 20. Backward Pass

The backward pass calculates LF and LS.

It begins at the project finish and moves backward toward the project start.

## 20.1 Backward Pass Rules

For each ending activity:

    LF = Project completion time

For every activity:

    LS = LF - Duration

If an activity has more than one successor:

    LF = Minimum LS of all immediate successors

The minimum is used because the activity must finish early enough for every successor to begin on time.

## Memory Rule

> Backward pass means subtract and take the minimum.

---

## 20.2 Activities F and G

F and G are ending activities.

The project completion time is 32 weeks.

### Activity F

    LF of F = 32
    LS of F = 32 - 6
    LS of F = 26

### Activity G

    LF of G = 32
    LS of G = 32 - 5
    LS of G = 27

Therefore:

| Activity |  LS |  LF |
| :------- | --: | --: |
| F        |  26 |  32 |
| G        |  27 |  32 |

Activity G finishes as early as week 31 but may finish as late as week 32 without delaying the project.

---

## 20.3 Activity E

Activity E has two immediate successors:

- Activity F
- Activity G

Their latest start times are:

    LS of F = 26
    LS of G = 27

Activity E must finish in time for both successors.

Therefore, use the smaller value.

    LF of E = Minimum of 26 and 27
    LF of E = 26

Activity E has a duration of 9 weeks.

    LS of E = 26 - 9
    LS of E = 17

Therefore:

| Activity |  LS |  LF |
| :------- | --: | --: |
| E        |  17 |  26 |

---

## 20.4 Activity D

Activity D has one successor, Activity E.

    LF of D = LS of E
    LF of D = 17

Activity D has a duration of 8 weeks.

    LS of D = 17 - 8
    LS of D = 9

Therefore:

| Activity |  LS |  LF |
| :------- | --: | --: |
| D        |   9 |  17 |

---

## 20.5 Activity C

Activity C has one successor, Activity F.

    LF of C = LS of F
    LF of C = 26

Activity C has a duration of 12 weeks.

    LS of C = 26 - 12
    LS of C = 14

Therefore:

| Activity |  LS |  LF |
| :------- | --: | --: |
| C        |  14 |  26 |

---

## 20.6 Activity A

Activity A has two successors:

- Activity C
- Activity D

Their latest start times are:

    LS of C = 14
    LS of D = 9

Activity A must finish early enough for both successors.

Therefore, use the smaller value.

    LF of A = Minimum of 14 and 9
    LF of A = 9

Activity A has a duration of 7 weeks.

    LS of A = 9 - 7
    LS of A = 2

Therefore:

| Activity |  LS |  LF |
| :------- | --: | --: |
| A        |   2 |   9 |

---

## 20.7 Activity B

Activity B has one successor, Activity D.

    LF of B = LS of D
    LF of B = 9

Activity B has a duration of 9 weeks.

    LS of B = 9 - 9
    LS of B = 0

Therefore:

| Activity |  LS |  LF |
| :------- | --: | --: |
| B        |   0 |   9 |

---

# 21. Complete CPM Results

| Activity | Duration |  ES |  EF |  LS |  LF | Slack |
| :------- | -------: | --: | --: | --: | --: | ----: |
| A        |        7 |   0 |   7 |   2 |   9 |     2 |
| B        |        9 |   0 |   9 |   0 |   9 |     0 |
| C        |       12 |   7 |  19 |  14 |  26 |     7 |
| D        |        8 |   9 |  17 |   9 |  17 |     0 |
| E        |        9 |  17 |  26 |  17 |  26 |     0 |
| F        |        6 |  26 |  32 |  26 |  32 |     0 |
| G        |        5 |  26 |  31 |  27 |  32 |     1 |

---

# 22. Calculating Slack

Slack can be calculated with either formula:

    Slack = LS - ES

or:

    Slack = LF - EF

Both formulas should produce the same answer.

## 22.1 Activity A

    Slack of A = LS - ES
    Slack of A = 2 - 0
    Slack of A = 2 weeks

Check using the other formula:

    Slack of A = LF - EF
    Slack of A = 9 - 7
    Slack of A = 2 weeks

Activity A can be delayed by up to 2 weeks without delaying the project.

## 22.2 Activity B

    Slack of B = 0 - 0
    Slack of B = 0 weeks

Activity B is critical.

## 22.3 Activity C

    Slack of C = 14 - 7
    Slack of C = 7 weeks

Activity C can begin as early as week 7 or as late as week 14.

It can finish as early as week 19 or as late as week 26.

## 22.4 Activity D

    Slack of D = 9 - 9
    Slack of D = 0 weeks

Activity D is critical.

## 22.5 Activity E

    Slack of E = 17 - 17
    Slack of E = 0 weeks

Activity E is critical.

## 22.6 Activity F

    Slack of F = 26 - 26
