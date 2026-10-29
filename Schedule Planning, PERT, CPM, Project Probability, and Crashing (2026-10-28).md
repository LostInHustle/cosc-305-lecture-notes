# Schedule Planning, PERT, CPM, Project Probability, and Crashing

## Reference Lecture Notes

## 1. Overview

This lecture continues the study of project schedule planning. The main topics are:

1. Reviewing the Critical Path Method
2. Creating a project network
3. Completing the forward and backward passes
4. Calculating slack
5. Identifying the critical path
6. Using PERT when activity durations are uncertain
7. Calculating expected activity times and variances
8. Estimating the probability of meeting a project deadline
9. Shortening a schedule through crashing
10. Comparing normal project cost with crashed project cost
11. Including recurring project costs in the final decision

The central idea is that project managers must understand both time and cost. A schedule may look reasonable during planning, but delays can occur during execution. The project manager must then decide whether to accept the delay, add resources, overlap activities, or pay to shorten the schedule.

---

# Part I: Critical Path Method

## 2. What Is CPM?

The Critical Path Method, or CPM, is a scheduling method used when activity times are treated as known and deterministic.

A deterministic duration means that one duration is assigned to each activity. For example, if an activity is expected to take six days, CPM uses six days as its duration.

CPM helps a project manager determine:

- The order in which activities must occur
- The earliest time each activity can begin
- The earliest time each activity can finish
- The latest time each activity can begin without delaying the project
- The latest time each activity can finish without delaying the project
- The amount of slack available for each activity
- The total expected project duration
- The critical path

---

## 3. Information Needed to Create a CPM Network

A CPM network normally begins with a table containing:

- Activity number or activity name
- Immediate predecessor or predecessors
- Activity duration

An immediate predecessor is an activity that must be completed before another activity can begin.

For example:

- Activity 1 has no predecessor, so it may begin immediately.
- Activity 3 has Activity 1 as its predecessor, so Activity 3 cannot begin until Activity 1 is complete.
- Activity 7 has Activities 5 and 6 as predecessors, so both must be complete before Activity 7 may begin.

The predecessor relationships determine the shape of the project network.

---

## 4. Creating the Network Diagram

The lecture example used the following general relationships:

1. Activities 1 and 2 begin at the start of the project.
2. Activity 3 follows Activity 1.
3. Activity 4 follows Activity 2.
4. Activity 5 follows Activity 3.
5. Activity 6 follows Activities 1 and 4.
6. Activity 7 follows Activities 5 and 6.
7. Activity 8 follows Activity 7.
8. Activity 9 follows Activity 8.
9. Activity 10 also follows Activity 8.
10. Activity 11 follows Activities 9 and 10.

A simple text representation is:

Start → Activity 1 → Activity 3 → Activity 5  
Start → Activity 2 → Activity 4 → Activity 6  
Activities 5 and 6 → Activity 7 → Activity 8  
Activity 8 → Activities 9 and 10  
Activities 9 and 10 → Activity 11 → Finish

When two or more activities lead into the same activity, the following activity must wait for all required predecessors.

---

# Part II: Forward Pass

## 5. Purpose of the Forward Pass

The forward pass determines:

- Earliest Start, written as ES
- Earliest Finish, written as EF
- Total expected project duration

The calculations move from the beginning of the network toward the end.

---

## 6. Forward Pass Formulas

For the first activity:

**ES = 0**

For every activity:

**EF = ES + t**

where:

**t = activity duration**

If an activity has one predecessor:

**ES(activity) = EF(predecessor)**

If an activity has multiple predecessors:

**ES(activity) = max(EF₁, EF₂, …, EFₙ)**

The maximum is used because the activity cannot begin until every required predecessor has finished.

---

## 7. Forward Pass Example

Suppose an activity begins at time 0 and takes six weeks.

**ES = 0**

**EF = 0 + 6 = 6**

If the next activity takes three weeks:

**ES = 6**

**EF = 6 + 3 = 9**

If another activity has two predecessors that finish at weeks 11 and 13:

**ES = max(11, 13) = 13**

The activity must wait until week 13 because that is when both predecessors have been completed.

In the lecture example, the final earliest finish was:

**EF(project) = 24**

Therefore, the total planned project duration was 24 time units.

---

# Part III: Backward Pass

## 8. Purpose of the Backward Pass

The backward pass determines:

- Latest Finish, written as LF
- Latest Start, written as LS

The calculations begin at the end of the network and move backward toward the start.

The latest times show how late an activity may occur without delaying the project.

---

## 9. Backward Pass Formulas

For the final activity:

**LF = project duration**

For every activity:

**LS = LF - t**

If an activity has one successor:

**LF(activity) = LS(successor)**

If an activity has multiple successors:

**LF(activity) = min(LS₁, LS₂, …, LSₙ)**

The minimum is used because the activity must finish early enough to avoid delaying any successor.

---

## 10. Why the Backward Pass Uses the Minimum

The forward pass uses the maximum because an activity must wait for all its predecessors.

The backward pass uses the minimum because an activity must finish before the earliest required start among all its successors.

This is one of the most important distinctions to remember:

- Forward pass with multiple predecessors: use the maximum.
- Backward pass with multiple successors: use the minimum.

---

# Part IV: Slack and the Critical Path

## 11. What Is Slack?

Slack is the amount of time an activity can be delayed without delaying the entire project.

Slack may be calculated using either of these equations:

**Slack = LS - ES**

or

**Slack = LF - EF**

Both equations should produce the same result.

---

## 12. Interpreting Slack

If:

**Slack = 0**

the activity is critical.

If:

**Slack > 0**

the activity has some scheduling flexibility.

For example, if an activity has:

**ES = 4**

and:

**LS = 6**

then:

**Slack = 6 - 4 = 2**

The activity may be delayed by two time units without delaying the project, assuming nothing else changes.

---

## 13. The Critical Path

The critical path is the longest duration path from the beginning of the project to the end.

It is also the path consisting of activities with zero slack.

In the lecture example, the critical path was:

**1 → 3 → 5 → 7 → 8 → 9 → 11**

These activities require close attention because any delay in one of them will normally delay the entire project.

A project may have more than one critical path. This occurs when two or more complete paths have the same longest duration.

---

## 14. A Quick Method for Comparing Parallel Paths

When two paths operate in parallel between the same points, the longer path controls the schedule through that portion of the network.

For example:

Path 1:

**8 → 9 → 11**

Path 2:

**8 → 10 → 11**

The path with the longer total duration is more likely to be critical.

This shortcut is useful for simple networks. For complicated networks, complete the full forward and backward pass because activities may reconnect in ways that are not immediately obvious.

---

## 15. Common CPM Errors

Common calculation errors include:

- Adding the wrong activity duration
- Using the minimum instead of the maximum during the forward pass
- Using the maximum instead of the minimum during the backward pass
- Forgetting that all predecessors must be completed
- Subtracting the wrong duration during the backward pass
- Identifying a path as critical without checking its total duration
- Assuming there can be only one critical path
- Treating an activity with positive slack as critical

A final reasonableness check is important. If the numbers do not agree with the structure of the network, review the calculations.

---

# Part V: PERT

## 16. What Is PERT?

PERT stands for Program Evaluation and Review Technique.

PERT is useful when activity durations are uncertain. Instead of assigning only one duration to an activity, PERT uses three estimates:

1. Optimistic time
2. Most likely time
3. Pessimistic time

PERT converts these three estimates into one expected activity time.

---

## 17. The Three PERT Time Estimates

### Optimistic time

The optimistic time, represented by \(a\), is the shortest realistic duration if conditions are highly favourable.

### Most likely time

The most likely time, represented by \(m\), is the duration expected under normal conditions.

### Pessimistic time

The pessimistic time, represented by \(b\), is the longest realistic duration if significant problems occur.

The pessimistic estimate should represent a difficult but plausible situation, not an impossible worst case.

---

## 18. Expected Activity Time

The expected time for an activity is:

**tₑ = (a + 4m + b) / (6)**

where:

**a = optimistic time**

**m = most likely time**

**b = pessimistic time**

The most likely estimate receives four times as much weight as either the optimistic or pessimistic estimate.

### Example

Suppose:

**a = 3**

**m = 5**

**b = 9**

Then:

**tₑ = (3 + 4(5) + 9) / (6)**

**tₑ = (3 + 20 + 9) / (6)**

**tₑ = (32) / (6)**

**tₑ = 5.33**

The expected activity time is approximately 5.33 time units.

---

## 19. Activity Variance

The variance of an activity is:

**σ² = ((b-a) / (6))²**

The standard deviation is:

**σ = (b-a) / (6)**

Variance measures the uncertainty associated with the activity duration.

A larger difference between the optimistic and pessimistic estimates produces a larger variance.

### Example

Using:

**a = 3**

and:

**b = 9**

the variance is:

**σ² = ((9-3) / (6))²**

**σ² = 1²**

**σ² = 1**

---

## 20. Moving from PERT to a Project Network

After calculating the expected time for every activity, use those expected times as the durations in the network.

The remaining schedule analysis resembles CPM:

1. Create the network.
2. Insert the expected activity times.
3. Calculate the duration of each path.
4. Identify the longest path.
5. Treat the longest path as the critical path.
6. Add the expected times on the critical path to estimate the total project time.

PERT adds probability and uncertainty, but the network logic remains similar to CPM.

---

# Part VI: Project Mean and Variance

## 21. Expected Project Duration

The expected project duration is the sum of the expected activity times on the critical path:

**μₚ = Σ(i in CP) t(e,i)**

where:

**μₚ = expected project duration**

**CP = critical path**

Only activities on the identified critical path are included in this calculation.

In the lecture example, the critical path was:

**A → D → F**

The expected project duration was:

**μₚ = 20.5**

Therefore, the project was expected to take 20.5 weeks.

---

## 22. Project Variance

Under the standard PERT assumptions, the project variance is estimated by adding the activity variances along the critical path:

**σₚ² = Σ(i in CP)σᵢ²**

The project standard deviation is:

**σₚ = √(σₚ²)**

In the lecture example:

**σₚ ≈ 1.848**

This standard deviation is used to calculate the probability of meeting a deadline.

---

## 23. Important PERT Assumptions

The standard PERT calculation makes several simplifying assumptions:

- Activity durations are treated as independent.
- The critical path is assumed to remain unchanged.
- Expected times are approximated using three estimates.
- The total project duration is approximated using a normal distribution.
- Variances are added only along the critical path.

In a real project, activity durations may be correlated, and the critical path may change. Therefore, PERT provides an estimate, not a guarantee.

---

# Part VII: Probability of Meeting a Deadline

## 24. Normal Distribution Approximation

PERT commonly approximates the total project duration with a normal distribution.

The distribution is centred at the expected project duration:

**μₚ = 20.5**

If the deadline equals the mean, the approximate probability of finishing by that deadline is:

**P(T ≤ μₚ) = 0.50**

Therefore, a deadline equal to the expected project duration does not represent a highly confident commitment. It represents approximately a 50 percent probability under the normal approximation.

---

## 25. The Z Score

To calculate the probability of completing the project by a target deadline, convert the deadline to a standard normal Z score:

**Z = (T-μₚ) / (σₚ)**

where:

**T = target completion time**

**μₚ = expected project duration**

**σₚ = project standard deviation**

---

## 26. Probability Example

Suppose:

**T = 25**

**μₚ = 20.5**

**σₚ = 1.848**

Then:

**Z = (25-20.5) / (1.848)**

**Z = (4.5) / (1.848)**

**Z ≈ 2.43**

A cumulative standard normal table gives approximately:

**P(Z ≤ 2.43) ≈ 0.9925**

Therefore:

**P(T ≤ 25) ≈ 99.25%**

The estimated probability of completing the project within 25 weeks is approximately 99.25 percent.

---

## 27. Interpreting Probability Results

If the target deadline is:

- Equal to the mean, the probability is approximately 50 percent.
- Greater than the mean, the probability is greater than 50 percent.
- Less than the mean, the probability is less than 50 percent.

This provides a quick reasonableness check before using the Z table.

For example, if the expected duration is 20.5 weeks and the deadline is 25 weeks, the answer must be greater than 50 percent. If a calculation produces 49 percent, the wrong section of the Z table was probably used.

---

## 28. Different Types of Z Tables

Standard normal tables may report different areas.

### Cumulative table

This table reports:

**P(Z ≤ z)**

It gives the area from negative infinity to a selected Z value.

For:

**Z = 2.43**

the cumulative probability is approximately:

**0.9925**

### Mean to Z table

This table reports the area between:

**Z = 0**

and the selected positive Z value.

For:

**Z = 2.43**

the area is approximately:

**0.4925**

To calculate the cumulative probability, add 0.5:

**0.5 + 0.4925 = 0.9925**

The final probability is:

**99.25%**

Always read the heading or diagram attached to the table before using its values.

---

## 29. Other Probability Questions

### Probability of finishing before a deadline

**P(T ≤ t)**

Find the Z score and use the cumulative probability.

### Probability of finishing after a deadline

**P(T > t) = 1 - P(T ≤ t)**

### Probability of finishing between two deadlines

**P(t₁ ≤ T ≤ t₂)**

Calculate two Z scores:

**Z₁ = (t₁-μₚ) / (σₚ)**

**Z₂ = (t₂-μₚ) / (σₚ)**

Then subtract the cumulative probabilities:

**P(t₁ ≤ T ≤ t₂) = P(Z ≤ Z₂)-P(Z ≤ Z₁)**

---

## 30. Reasonableness Checks

Before accepting a probability answer, ask:

- Is the deadline above or below the mean?
- Should the answer be above or below 50 percent?
- Is the deadline several standard deviations from the mean?
- Did I use variance or standard deviation in the Z formula?
- Did I use the correct section of the normal table?
- Does the final percentage fit the shape of the normal curve?

Do not place the variance directly into the Z formula. The denominator must be the standard deviation.

---

# Part VIII: Schedule Compression

## 31. Why a Schedule May Need to Be Shortened

A project can fall behind because:

- An activity takes longer than expected.
- Workers or equipment are unavailable.
- Materials arrive late.
- The customer changes a requirement.
- Rework becomes necessary.
- A regulatory approval is delayed.
- The original estimate was inaccurate.
- A new contractual deadline is introduced.

When a delay threatens the required completion date, the project manager may need to compress the schedule.

Two important schedule compression methods are:

1. Crashing
2. Fast tracking

---

## 32. Crashing

Crashing means reducing an activity’s duration by adding resources or using a more expensive method.

Examples include:

- Hiring additional workers
- Authorizing overtime
- Using faster equipment
- Paying for expedited delivery
- Adding another work shift
- Assigning a more experienced team
- Outsourcing part of the activity

Crashing normally increases direct project cost.

---

## 33. Fast Tracking

Fast tracking means performing activities in parallel that were originally planned in sequence.

For example, a team may begin part of the implementation before every design detail is complete.

Fast tracking can reduce project duration, but it may create:

- Additional coordination requirements
- Greater rework risk
- Communication problems
- Quality problems
- Dependency conflicts

Crashing primarily adds resources or cost. Fast tracking primarily changes the sequence or overlap of work.

---

# Part IX: Crashing Calculations

## 34. Information Required for Crashing

For each activity, the project manager needs:

- Normal time
- Crash time
- Normal cost
- Crash cost
- Maximum possible time reduction
- Crash cost per time unit

### Normal time

The duration under ordinary working conditions.

### Crash time

The shortest realistic duration after additional resources or faster methods are used.

### Normal cost

The direct cost of completing the activity in its normal time.

### Crash cost

The direct cost of completing the activity in its crash time.

---

## 35. Maximum Number of Crash Days

The maximum number of days an activity may be shortened is:

**Maximum crash days = Normal time - Crash time**

### Example

If:

**Normal time = 5**

and:

**Crash time = 3**

then:

**Maximum crash days = 5 - 3 = 2**

The activity may be shortened by no more than two days.

---

## 36. Crash Cost Per Day

The crash cost per day is:

**Crash cost per day = \fracCrash cost-Normal cost Normal time-Crash time**

This value is also called the crash slope.

### Example

Suppose:

**Normal time = 5**

**Crash time = 3**

**Normal cost = $4,000**

**Crash cost = $5,000**

The maximum reduction is:

**5 - 3 = 2 days**

The additional cost is:

**$5,000 - $4,000 = $1,000**

Therefore:

**Crash cost per day = ($1,000) / (2) = $500**

It costs an additional $500 for each day removed from the activity.

---

## 37. General Crashing Procedure

Use the following process:

1. Draw the project network.
2. Calculate the duration of every complete path.
3. Identify the current critical path or paths.
4. Find crashable activities on the critical path.
5. Select the least expensive valid crashing option.
6. Reduce the selected activity by one time unit.
7. Recalculate all path durations.
8. Identify the new critical path or paths.
9. Repeat until the target duration is reached or no further crashing is possible.

The network must be recalculated after each crashing decision because the critical path can change.

---

# Part X: Crashing with Multiple Critical Paths

## 38. Why Multiple Critical Paths Matter

If the project has two critical paths, reducing an activity on only one path may not reduce the total project duration.

Suppose two critical paths are both 20 days long.

If an activity unique to the first path is shortened by one day:

- The first path becomes 19 days.
- The second path remains 20 days.
- The project duration remains 20 days.

Money has been spent, but the project has not been shortened.

---

## 39. Valid Options with Multiple Critical Paths

To shorten a project with multiple critical paths, the manager must either:

1. Crash one activity shared by all critical paths, or
2. Crash a separate activity on each critical path at the same time

The total cost of option 2 is the combined crash cost of the selected activities.

### Example

Suppose Activity D is on the first critical path and costs $500 per day to crash.

Activity E is on the second critical path and costs $1,000 per day to crash.

To shorten both paths by one day:

**$500 + $1,000 = $1,500**

If Activity B is shared by both critical paths and costs $750 per day to crash, Activity B is the less expensive choice:

**$750 < $1,500**

Therefore, crashing Activity B is the better decision.

---

## 40. Lecture Crashing Sequence

The project initially had two critical paths with durations of 20 days.

A shorter path had a duration of 17 days.

The crashing sequence was approximately:

1. Crash Activity G by one day at $250.
2. Crash Activity G by another day at $250.
3. Crash Activity B by one day at $750.
4. Crash Activities D and E together by one day at a combined cost of $1,500.
5. Crash Activities D and E together by another day at a combined cost of $1,500.

The total additional crashing cost was:

**$250 + $250 + $750 + $1,500 + $1,500**

**= $4,250**

The project duration was reduced from 20 days to 15 days.

---

## 41. Total Direct Cost After Crashing

Suppose the normal direct project cost is:

**$18,450**

The additional crashing cost is:

**$4,250**

The total direct cost after crashing is:

**$18,450 + $4,250 = $22,700**

Crashing increases direct project cost because additional resources are used to reduce the schedule.

---

# Part XI: Recurring Project Costs

## 42. Fixed Cost Per Project Day

Some project costs continue for every day the project remains active.

Examples include:

- Equipment rental
- Site office rental
- Temporary facilities
- Software licences
- Security
- Utilities
- Project management staff
- Insurance
- Supervision
- Daily administrative expenses

Assume the recurring project cost is:

**$1,000 per day**

---

## 43. Normal Schedule Cost with Recurring Costs

If the normal duration is 20 days:

**20 × $1,000 = $20,000**

Add this to the normal direct cost:

**$18,450 + $20,000 = $38,450**

Therefore, the total cost of the normal 20 day schedule is:

**$38,450**

---

## 44. Crashed Schedule Cost with Recurring Costs

The crashed direct cost is:

**$22,700**

The crashed project duration is 15 days.

The recurring cost is:

**15 × $1,000 = $15,000**

Therefore:

**$22,700 + $15,000 = $37,700**

The total cost of the crashed schedule is:

**$37,700**

---

## 45. Cost Comparison

Normal 20 day schedule:

**$38,450**

Crashed 15 day schedule:

**$37,700**

Difference:

**$38,450 - $37,700 = $750**

In this example, crashing the project reduces the total cost by $750.

This happens because the $5,000 reduction in recurring costs is greater than the $4,250 increase in direct crashing costs.

The net saving is:

**$5,000 - $4,250 = $750**

Crashing does not always increase total project cost. It increases direct cost, but it may reduce recurring or indirect costs enough to lower the overall cost.

---

# Part XII: Time and Cost Tradeoff

## 46. Direct and Indirect Costs

### Direct costs

Direct costs are associated with completing individual activities.

They may include:

- Labour
- Materials
- Equipment
- Overtime
- Expedited delivery
- Contractor fees

Direct costs usually increase when a project is crashed.

### Indirect or recurring costs

Indirect costs relate to keeping the overall project operating.

They may include:

- Office rental
- Supervision
- Administration
- Insurance
- Security
- Temporary facilities
- General overhead

Indirect costs generally decrease when the project duration is reduced.

---

## 47. Minimum Cost Schedule

The minimum cost schedule is the project duration that produces the lowest total cost.

Conceptually:

**Total project cost = Direct cost + Indirect cost**

As the schedule is shortened:

- Direct cost usually rises.
- Indirect cost usually falls.

The best schedule is not automatically the shortest schedule. It is the schedule that meets the project’s requirements at the most appropriate total cost and risk level.

---

# Part XIII: Important Exam and Assignment Lessons

## 48. CPM Checklist

For a CPM problem:

1. List all activities.
2. Identify immediate predecessors.
3. Draw the network.
4. Insert activity durations.
5. Complete the forward pass.
6. Use the maximum when predecessors merge.
7. Determine the total project duration.
8. Complete the backward pass.
9. Use the minimum when successors separate.
10. Calculate slack.
11. Identify all zero slack activities.
12. Confirm the critical path.

---

## 49. PERT Checklist

For a PERT problem:

1. Record the optimistic estimate.
2. Record the most likely estimate.
3. Record the pessimistic estimate.
4. Calculate the expected time for each activity.
5. Calculate the variance for each activity.
6. Build the network using expected times.
7. Identify the critical path.
8. Add expected times on the critical path.
9. Add variances on the critical path.
10. Take the square root of project variance.
11. Calculate the Z score.
12. Use the correct normal table.
13. Check whether the probability is logically reasonable.

---

## 50. Crashing Checklist

For a crashing problem:

1. Calculate the normal duration of every path.
2. Identify all critical paths.
3. Calculate crash cost per day for every activity.
4. Consider only activities on the current critical path or paths.
5. Select the least expensive valid option.
6. If there are multiple critical paths, shorten all of them.
7. Crash incrementally.
8. Recalculate all path durations after every decision.
9. Track the remaining crash capacity of every activity.
10. Stop when the target duration is reached.
11. Add the crashing cost to the normal direct cost.
12. Include recurring costs when required.
13. Compare total costs before choosing the final schedule.

---

# Part XIV: Common Mistakes

## 51. CPM Mistakes

- Using the wrong predecessor relationship
- Forgetting one branch of the network
- Using the minimum during the forward pass
- Using the maximum during the backward pass
- Calculating slack using mismatched values
- Assuming the visually longest path is automatically critical
- Ignoring a second critical path

---

## 52. PERT Mistakes

- Using three estimates without applying the PERT formula
- Forgetting the weight of four on the most likely time
- Forgetting to square the variance expression
- Adding standard deviations instead of variances
- Using variance instead of standard deviation in the Z formula
- Including variances from activities outside the critical path
- Reading the wrong area from the normal table
- Reporting 0.4925 instead of 0.9925 for a positive Z score of 2.43 when using a mean to Z table

---

## 53. Crashing Mistakes

- Crashing a noncritical activity
- Selecting the cheapest activity in the entire network instead of the cheapest valid activity on the critical path
- Crashing one of two critical paths while leaving the other unchanged
- Forgetting that the critical path can change
- Exceeding an activity’s maximum crash capacity
- Failing to update activity durations
- Ignoring recurring project costs
- Assuming the shortest schedule must have the lowest total cost

---

# Part XV: Formula Summary

## CPM formulas

**EF = ES + t**

**LS = LF - t**

**Slack = LS - ES**

**Slack = LF - EF**

For multiple predecessors:

**ES = max(EF₁, EF₂, …, EFₙ)**

For multiple successors:

**LF = min(LS₁, LS₂, …, LSₙ)**

## PERT expected time

**tₑ = (a + 4m + b) / (6)**

## PERT variance

**σ² = ((b-a) / (6))²**

## Expected project duration

**μₚ = Σ(i in CP) t(e,i)**

## Project variance

**σₚ² = Σ(i in CP)σᵢ²**

## Project standard deviation

**σₚ = √(σₚ²)**

## Z score

**Z = (T-μₚ) / (σₚ)**

## Maximum crash reduction

**Maximum crash time = Normal time - Crash time**

## Crash cost per day

**Crash cost per day = \fracCrash cost-Normal cost Normal time-Crash time**

## Total project cost

**Total cost = Direct cost + Indirect or recurring cost**

---

# Final Summary

CPM is used to organize activities with known durations and identify the longest path through a project. The forward pass calculates earliest times, while the backward pass calculates latest allowable times. Activities with zero slack form the critical path.

PERT extends network scheduling by recognizing uncertainty. It uses optimistic, most likely, and pessimistic estimates to calculate expected activity times and variances. The expected times on the critical path determine the estimated project duration. The variances on the critical path are added to estimate the project variance. A Z score can then be used to estimate the probability of meeting a deadline.

When the schedule must be shortened, the project manager may use crashing or fast tracking. Crashing adds resources and usually increases direct cost. Fast tracking overlaps activities and may increase risk and rework.

Crashing decisions must focus on the current critical path. If several critical paths exist, all of them must be shortened for the total project duration to decrease. Recurring daily costs must also be considered because a shorter schedule can sometimes reduce the total project cost, even when direct crashing costs increase.
