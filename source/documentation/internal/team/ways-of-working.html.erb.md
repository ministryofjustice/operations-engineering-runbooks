---
owner_slack: "#operations-engineering-alerts"
title: Ways of Working
last_reviewed_on: 2025-02-17
review_in: 3 months
---

# Ways of Working

This document serves as our collaborative playbook, providing clear guidelines and standardised processes for 'how we
work' together. It ensures consistency, clarity, and efficiency in our daily tasks, fostering a harmonious team culture.
By referring to this document, we align ourselves toward common goals, resolve conflicts, and adapt to changing needs.
It's not just a set of rules; it's a tool for continuous improvement, helping us evolve and excel as a team.

**Statuses:**

- ✅ Accepted
- 🧪 Experimenting
- 💡 New idea (waiting to be discussed by the team)
- ⏸️ Paused (due to another active experiment)

## **Delivery**

### **✅ We Update Stories With Progress**

To increase team awareness of progress and/or updates on a specific ticket, we are experimenting with updating tickets using the comment section on the issue itself. This applies when:

- New information is discovered that may alter the acceptance criteria or functional requirements of a ticket.
- A team member has upcoming leave and is still working on a ticket, ensuring that when picked up by someone new a brief overview of the current status is passed on.

### **✅ We Use 2-Week Sprints**

2-week sprints have been accepted as a reasonable time frame to balance the need for the team to deliver complex work
items, and the need to include reflective practices such as demos, retrospectives, and sprint planning frequently.

### **✅ Implementing Firebreak Sprints**

We embrace Firebreak Sprints as a vital component of our engineering process, dedicating structured breaks from our regular sprint cycles to activities that significantly contribute to our technical health, innovation, and team well-being.

For inspiration and guidance, we look to the GOV.UK team's approach to Firebreak Sprints. Their experiences underscore the value of such initiatives in promoting technical excellence and team well-being. For more information, please see our documentation describing [Firebreak Sprints](https://runbooks.operations-engineering.service.justice.gov.uk/documentation/internal/firebreak-sprints.html).

### **✅ Sprint backlog contents**

The stories in a sprint backlog will depend on priorities, however we will always include stories from the following catagories:

- **sprint goal stories** - these will directly relate to roadmap priorities and form the majority of the sprint backlog.
- **refactor story** - at least one refactor story to ensure that our code is well maintained.
- **risk story**  - at least one story relating to items from our risk register.

### **✅ Archive Repository Once a Proof of Concept is Complete**

Once a Proof of Concept (POC) is complete, the associated GitHub repository should be removed from the [GitHub Repository Terraform](https://github.com/ministryofjustice/operations-engineering/tree/main/terraform/github/repositories), this will automatically archive the repository. This ensures that the repository estate is not polluted by lingering POC repositories.

### 💡 Set Quarterly Goals

Quarterly goals align our team's efforts with broader objectives and enhance our focus and productivity. These goals will be defined collaboratively with senior stakeholders and discussed with the team, reflecting our shared priorities and aspirations. By establishing clear, measurable targets, we aim to drive our team's progress, foster alignment, and celebrate achievements together.

Quarterly Goals are:

- ✅ SMART (Specific, Measurable, Achievable, Relevant, Time-bound)
- ✅ A tool to enable effective planning, tracking, and communication of our progress - we are still an agile team and will continue to adapt and respond to change
- ✅ A concise list of 3 goals that are achievable within the quarter
- ✅ Aligned with the team's overall objectives and priorities
- ✅ Regularly reviewed and updated to reflect our evolving needs and progress i.e. if a goal is completed early, we can add a new one or adjust existing goals as we learn more about our work

Quarterly Goals are not:

- ❌ A rigid set of targets that must be met at all costs
- ❌ A tool for de-prioritising business requirements or other priorities such as day-to-day operational work, addressing technical debt, administrative responsibilities and peoples personal learning and development time
- ❌ A vague statement of intent or aspiration without clear, measurable outcomes
- ❌ A static list that remains unchanged throughout the quarter - where we need to adapt our goals, we will do so and reflect on learning and insights gained
- ❌ An extensive list of goals that dilutes our focus and makes it difficult to track progress

> *Examples:*
>
> - A Good Delivery Goal - *"Improve tagging of AWS resources by increasing meaningful coverage by 20% by the end of the quarter"*
> - A Poor Delivery Goal - *"Improve AWS resource tagging"*
> - A Good Discovery Goal - *"Understand the top 3 saving oppurtunities within AWS, complete with risk assessments, potential savings oppurtunities and high-level a plan for implementation by end of the quarter"*
> - A Poor Discovery Goal - *"Understand AWS costs"*

#### Measuring Success

To emphasise the importance of making committed progress towards our goals, we will measure our success by how we manage to commit our time to goal and the progress we made towards it. Again, focus and dedication to the goal is key not the completion of the goal itself.

We will use the following categories to measure our success of our goals:

*🚀 Surpassed Expectations*

Outcome: The team hit/exceeded the intended target, achieving more than expected. This reflects not only focus but exceptional performance or favourable external circumstances. This serves as an opportunity to celebrate and reflect on the factors that contributed to this outcome.

*✅ Achieved Progress*

Outcome: The team met the goal as far as reasonably possible, given the circumstances. This is a normal and positive outcome, emphasizing focus, dedication and progress, despite external challenges.

*🙈 Underprioritised*

Outcome: The team was unable to give sufficient attention to the goal. This serves as an opportunity to analyze and reflect on the barriers that led to this outcome

## **Ceremonies**

### **✅ Backlog Refinement**

These sessions enable us to review, prioritise, and adapt our tasks. By fine-tuning upcoming work items, we ensure
clarity and focus. Backlog refinement promotes effective planning, enabling us to address potential challenges in
advance. These sessions foster collaboration, empowering team members to contribute ideas and clarify doubts. Through
these targeted discussions, we maintain a well-organized backlog. Engaging in backlog refinement enhances our readiness
for future sprints.

### **✅ Demos**

These sessions ensure transparency, collaboration, and rapid improvement. By showcasing completed work to stakeholders,
we align everyone with our progress and gather immediate feedback. This process fosters team pride and accountability.
Additionally, demos empower stakeholders with direct insights, enhancing their engagement. Through these efficient
sessions, we celebrate successes, pinpoint areas for growth, and pivot effectively for upcoming sprints, ensuring our
continuous development and team cohesion.

### **✅ Milestone Planning**

To manage and deliver larger, more complex projects, we dedicate focused planning sessions for each phase of our Agile delivery process. These sessions are structured around specific delivery phases—Discovery, Alpha, Beta, Live, and Retirement—each represented by a dedicated milestone in our GitHub repository.

1. Dedicated Milestones for Each Phase: We create a separate milestone for each delivery phase in GitHub, ensuring transparent tracking and accountability for all tasks and objectives associated with that phase.

2. Planning for Future Phases: After establishing the tasks for the current milestone, we look ahead to upcoming phases. This proactive approach allows us to anticipate future needs and align our efforts accordingly, ensuring smooth transitions between phases.

3. Fostering Collaboration and Inclusion: These planning sessions are designed to be inclusive, giving every team member a voice in the process. Engaging all team members early enhances collaboration, gathers diverse insights, and ensures alignment on our shared goals.

#### Meeting Structure

Below is a suggested structure for the milestone planning meetings. This can evolve over time as we find a system that works best for the team:

1. **Review Full Milestone List (~10 Minutes):**:
   Review the full list of Operations Engineering [milestones](https://github.com/ministryofjustice/operations-engineering/milestones). Some milestones are hidden from the [default list](https://github.com/orgs/ministryofjustice/projects/52/views/11) due to no active stories being allocated to them.

   This section of the meeting is to confirm that the team is still happy with their state, and whether additional tickets are needed to bring these into the active milestone section.

2. **Initial Ticket Sort (~40 Minutes):**:
   Starting from the top of the active milestone list the team reviews the current list of tickets. Each ticket is confirmed by the team to be an essential part of the work needed to complete the milestone.

   Once completed, we add any relevant stories from the backlog that currently have no milestones assigned, and create new stories should we feel further work is needed. These stories are not to be filled out in detail, and act only as placeholders until the team's refinement meeting.

   For this section we need to take into consideration the stage of the milestone (alpha, beta, etc) when deciding on the work that is required.

3. **Milestone Progress Overview (~10 Minutes):**:
   The team performs a final review of the active milestones to ensure we are happy that everything in progress is relevant. This is an opportunity to close off milestones that are complete or are no longer relevant to the team.

### **✅ Retrospectives**

Retrospectives are pivotal in our team's evolution. These condensed and insightful sessions provide a dedicated space
for reflection, learning, and growth. By analysing our recent sprint, we identify successes and challenges, enabling us
to celebrate achievements and address obstacles. Retrospectives foster open communication, empowering team members to
share ideas for improvement candidly. Through these focused discussions, we refine our strategies, enhance
collaboration, and fortify our team dynamics. Embracing retrospectives ensures our continuous adaptation and drives us
toward excellence in every sprint.

To make it easier for anyone in the team to create a retrospective, we have included a 'Build-a-Retro' section on our [current board](https://miro.com/app/board/o9J_lsgfhYk=/). This is an area to improve over time with common components we feel help bring out the best of us in our retrospectives, and to help decrease the time needed to create one from scratch.

### **✅ Risk Register Review**

These sessions provide a clear understanding of our current risks and serve as a platform to discuss both existing and
potential new challenges. By openly addressing these risks, we foster a team-wide awareness and encourage proactive
problem-solving. These discussions empower us to develop effective strategies, enhancing our preparedness and
adaptability. Our focus is not just on identifying problems but on finding collective solutions. Engaging in these
reviews ensures that our team is well-equipped to navigate uncertainties and confidently make informed decisions.

For further details on the ceremony, visit
the [Risk Review Meeting Process](https://runbooks.operations-engineering.service.justice.gov.uk/documentation/internal/risk-review.html)

### **✅ Sprint Planning**

Sprint planning will now be conducted in three stages to prepare our tickets for the upcoming sprint better and ensure all tasks are well-defined and aligned with our sprint goals. This structured approach aims to enhance clarity, collaboration, and effective use of time:

1. **Initial Sprint Planning Session (~10 minutes):**
   The first part of the meeting is a brief session led by the Project Manager. The goal is to provide an overview of the upcoming sprint and a rough sorting of the relevant tickets. This initial sort sets the direction and context for the sprint, aligning the team on high-level priorities and focus areas.

2. **Mob Refinement Session (1 - 2 hour(s)):**
   The second stage is a collaborative mobbing session where the team refines each task or topic. This session focuses on ensuring that tickets are well-sized, clearly defined, and have a solid definition of done. It is driven by team input to foster a comprehensive understanding of the work ahead and ensure everyone is aligned on the expectations and deliverables.

   **We should include a 10-minute break during this section of the meeting to allow for a quick recharge.**

3. **Final Sprint Planning and Prioritisation (~10 minutes):**
   In the final session, the team performs a detailed sorting and prioritisation of all items proposed for the sprint. This stage considers constraints such as the number of staff available, the complexity of tasks, and the team’s understanding of each topic. This focused session ensures the sprint plan is realistic, achievable, and tailored to the team's capacity and expertise.

By breaking the sprint planning into these three distinct parts, we aim to improve preparation, reduce uncertainty, and optimise the time spent in planning. This approach also ensures that the team is well-prepared to tackle the sprint's tasks with clear expectations and a shared understanding.

### **✅ Emergency Sprint Planning**

In the event that we complete our sprint goal, and we have insufficient stories in the sprint backlog during a sprint we can call and emergency sprint planning session.

If an emergency planning session is called we should agree as a team whether to hold the session. We may want to consider risk or other stories from the backlog in the first instance.

The emergency planning will be a scalled down version of sprint planning, but follow the same format.

### **✅ Firebreak Sprint Planning**

When running a sprint planning session during a Firebreak, we aim to structure is as follows:

1. **Initial Sprint Planning Session (~10 minutes):**
   Much the same as regular planning, the first part of the meeting is a brief session led by the Project Manager. The goal is to provide an overview of the upcoming items in the Firebreak sprint and a rough sorting of the relevant tickets. We should also take some time here to briefly review the current Firebreak milestones to make sure the team is happy with their purpose and currently assigned tickets.

2. **Individual User Presentations (~30 minutes):**
   This section of the meeting gives each team member an opportunity to present their idea for a Firebreak story to the rest of the team. This will help ensure everyone understands what work is required to complete the story, and gives the team a changes to ask questions and challenge or suggest alternatives for the proposed approach.

   It's important here for the team to agree that the proposed Firebreak story is appropriately sized for the sprint.

3. **Firebreak Epics and Sub Issues (~20 minutes):**
   This portion of the meeting gives us some time to associate any new Firebreak stories with the appropriate Firebreak milestones. If a ticket is not relevant to a milestone, it can be brought in as a standalone story.

### **✅ Daily Stand-Up Meetings**

Our team holds daily stand-up meetings* in the morning to improve communication and collaboration. This consistent timing
aligns everyone, allowing for timely updates and obstacle resolution. Morning meetings enable efficient daily planning,
ensuring tasks are in sync with team objectives. This proactive approach enhances productivity and teamwork, making our
Agile process more effective.

The structure of the daily stand-up is:

- 🧪 We use a random name picker to determine who should facilitate the stand-up each day
- Discuss work completed
- Discuss work that is blocked
- Discuss work in progress
- While discussing work in progress, if the person who is working on the ticket is off for the entire day at stand-up, we move the ticket back into "To Do"
- Discuss work happening outside of the normal sprint board view

- *We skip the daily stand-up on the morning of Sprint Planning

#### **✅ If Unable to Attend Stand-Up, Post an Update in the Slack Channel**

Post a brief update in the designated Slack channel if you cannot attend stand-up. Sharing your progress, impediments,
and any help you need keeps the team informed and ensures we can support each other effectively, even when we're not
physically present.

### **✅ Stand-Down Reflections for Continuous Growth**

As we wrap up the day, let's reflect and share a moment in our Stand-Down thread. Post updates to celebrate
progress, voice frustrations to seek support, and highlight wins to spread joy. This transparency fosters teamwork and
growth.

- **Updates**: Please make sure to note what you've accomplished.
- **Frustrations**: Share any obstacles - remember, it's us against the problem.
- **Wins**: Let's cheer for our victories, big or small.

Stay constructive and kind.

### **✅ Ways of Engineering**

This ceremony is dedicated to discussing and reviewing our team's engineering practices in a structured yet open forum.
The goal is to foster continuous dialogue on improvements, innovations, and adjustments needed within our engineering domain.
This initiative will allow us to collectively assess the effectiveness of our current practices, explore new methodologies, and decide on the adoption of experimental practices on a regular basis. Participation and input from every team member are crucial for making this ceremony a valuable asset in our continuous improvement journey.

## General

### **✅ Team Socialisation**

We aim to partake in team social days at least every two months to ensure a healthy work-life balance and encourage
camaraderie through activities outside. These days are essential for us to step back from work and strengthen our team
dynamics through shared, informal experiences. We also aim to include virtual activities where we can help break up
some of the more ceremony-intense days.

For anyone wondering, Sam is currently the darts champion.<sup>[*citation needed*]</sup>

## Tools

### **✅ We use GitHub Projects For Project Workflow Visualisation**

To increase the visibility of our work in progress and to keep track/plan future work effectively, we use GitHub projects.

GitHub Projects is a simple-to-use project management tool that integrates seamlessly with our code repositories, which
are already hosted in GitHub.

It allows to easily add custom fields and metrics to keep track of project management related meta-data for work items,
and create specialised views to optimise our ceremonies.

Our board can be found [here](https://github.com/orgs/ministryofjustice/projects/52)

### **✅ Use Slack Huddles for all Ceremonies**

For all team ceremonies, we use Slack Huddles for the following reasons:

- Familiar with the tool as we it for daily communication
- Google is being decommissioned in the Ministry of Justice, so we want to move away depending on it
- Slack Huddles contains most features we need to effectively run most ceremonies

Where Slack Huddles is not suitable for a particular meeting, we can opt to use an alternative tool.

---

## Adding/Adjusting Ways of Working

Adding or adjusting our Ways of Working is a collaborative process. If you have a suggestion or think something needs to
change, raise a Pull Request to update the document! Feel free to discuss the change in our Slack channel or during our
Stand-Up. At latest, we'll discuss any changes during our Retrospective meetings. We value continuous improvement, so
your input is essential in shaping how we work together as a team.

### Experimental Ways of Working

As an innovative team, we're always exploring new methods to enhance our productivity and collaboration.

Remember, experiments are opportunities for us to learn and grow together. Your feedback and active participation are
vital in making these experiments successful.
