<!--- # Table of Contents

- [QA Workflow](#qa)
- [Development Workflow](#dev)
- [Change Management](#chg)
- [Design Package](#pkg)

# Execution

## Stages

1. Draft Definition
2. Project Champion(Business Owner)Review
3. Team member review 
4. Finalize and release workflow
5. Team members excute the released procedure

## Execution Feedback
- Comments on non-compliance
- Correction within 2 days following released standard
- New issues may be created for continious improvements

## Escalation
1. Facts collection
2. Refine definition
3. Management involvement
4. Suspending account in github if non-compliance can not be resolved within 7 days
5. Suspending project and archive repo if status cannot be maintained


# QA Workflow <a id="qa"></a>

Define status with time line and accountable assignee to track bugs or defects effectively during production stage.

- [QA Status](#qa-status)
- [Github Project Fields](#gh-field)

## QA Status <a id="qa-status"></a>
1. [Open](#qa-open)
2. [Triage](#qa-triage)
3. [Root Cause Analysis (RCA)](#qa-rca)
4. [Fix](#qa-fix)
5. [Done](#qa-done)

### Open <a id="qa-open"></a>
- Assignee: issue reporter
- Time block: 1 week
- Key information: 
  - Product Code
  - S/N
  - Precise bug or defect symptom
  - Tracking Number 

### Triage <a id="qa-triage"></a>
- Assignee: vendor QA lead
- Time block: 10 days
- Determine:
  - Assignee
  - Priority
  - Duplicates

### RCA <a id="qa-rca"></a>
- Assignee: vendor engineer
- Time block: depending on priority
- Key deliverables:
  - Vendor defect reports, or
  - Manufacture reports

### Fix <a id="qa-fix"></a>
- Assignee: vendor engineer
- Key deliverables:
  - Design changes, or
  - SOP changes
  - Pull request
  - Supporting documentation

### Done <a id="qa-done"></a>
- Assignee: issue reporter
- It's issue reporter's decision to close or not.

## Github Project Fields <a id="gh-field"></a>

- [Assignee](#gh-assignee)
- [Status](#gh-status)
- [Duplicate](#gh-duplicate)
- [Label](#gh-label)
- [Dates](#gh-date)

### Assignee <a id="gh-assignee"></a>
- A single person who is responsible for the current status

### Status <a id="gh-status"></a>
- A single select field to indicate status

### Duplicate <a id="gh-duplicate"></a>

- A text field to indicate this issue is a duplicate of another same issue. 
- Product Code: Issue ID

### Label <a id="gh-label"></a>

- A multi-select text field to indicate what are deliverables for this task or issue
- A report must be labelled when in RCA 
- Label can be used for many different purpose as long as definitions in one project are consistent 

### Open, RCA Start and Fix Date <a id="gh-date"></a>

- Date format fields to tracking time and status
- These field can also be used to generate meaningful performance indicator through filters, e.g. Q1 Open, Q2 Fix, etc. 


# Development Workflow <a id="dev"></a>

To be able to divide and conquer and track incremental changes during development stage

- [Task](#dev-task)
- [Trackor](#dev-trackor)
- [Assignee](#dev-assignee)
- [Priorities](#dev-priorities)
- [Status](#dev-status)
- [Area](#dev-area)
- [Deliverable](#dev-deliverable)
- [Timelines](#dev-timelines)

## Task <a id="dev-task"></a>

A single action item, e.g.

- Feature Request
- Bug Reports
- Test Case

A task may have a todo checklist.

## Trackor <a id="dev-trackor"></a>

A group of action items or sub trackors, e.g.

- Situation Appraisals
- Release Notes
- Test Plans

The rule of divide-and-conquer:
- A trackor must have a list of tasks or smaller trackors
- A trackor or a task must have deliverables defined or lablled

## Assignee <a id="dev-assignee"></a>

Each task or trackor must have a single person as assignee.

## Priorities <a id="dev-priorities"></a>

A ranking of importance and urgency

- High
- Medium
- Low

## Status <a id="dev-status"></a>

Indicate what is the current stage of a specific trackor or task

1. Open
2. Triage
3. Progess
4. Review
5. Done
6. Backlog

## Area <a id="dev-area"></a>

Functional domain of trackors or tasks,e.g
- PRODUCT
- ID
- SW
- HW
- MEC
- TEST
- QA
- PRODUCTION
- MARKETING

## Deliverable <a id="dev-deliverable"></a>

Results of tasks or trackors. All deliverables are certain format of documents, e.g.
- bin: s/w release binaries
- howto: tutorials
- id
- sw: s/w source code
- scripts
- sch: schematic
- pcb
- bom
- bom:cost
- mec
- test:plan
- test:rst 
- test:tc
- doc: prd, mkt

## Timelines <a id="dev-timelines"></a>

Short term and long term goals,

- Roadmap
- Milestone
- Sprint
- Start date and target date

## Risk <a id="dev-risk"></a>

Risk should be assessed on a trackor or task with timeline, especially a critical path. And it should be regularly updated.

- On Track
- At Risk
- Blocked

# Change Management <a id="chg"></a>

## General Guideline

Changes should be managed in an increasingly, more and more restrictive manner with more milestone achieved.

- Initially duing development, it serves more of a personal tracking tool for developers to exploring ideas and easily going back when ideas fail.
- After prototypes work, it serves more of building tool for developers to keeping building more things without breaking existing or impacting others.
- During preproduction or production stage, changes must be managed strictly to ensure solving problems not creating new problems or disastors.

- [ ] commit message
- [ ] branch
- [ ] reviews

## Design Package <a id="pkg"></a>

- [ ] folders
- [ ] releases


# Github Howtos and Admin

## Project Board <a id="howto-project"> </a>

- [Docs](https://docs.github.com/en/issues/trying-out-the-new-projects-experience/quickstart)
- Navigation
- Field
- Views
- Filters

## Markdown <a id="howto-md"></a>

# Folder Structure and Ownership



Folder | Description | Supplier Owner| FP Owner
-- | -- | -- | --
bin/ | software binaries | - | Champion
bom/ | list of all components | - | Champion
cert/ | compliance certificates | - | Champion
datasheet/ | component datasheets | - | Champion
flow/ | firmware flowchart| - | Champion
gfx/ | on-product graphics | - | Champion
mec/ | assemblies and custom parts | - | Champion
pcb/ | pcb/schematics | - | Champion
print/ | packaging and inserts | - | Champion
qa/ | quality assurance | - | Champion
sop/ | manufacturing procedures | - | Champion
spec/ | purchased part datasheets | - | Champion
test/ | cases, plans, and results | - | Champion
tr/ | technical requirements | - | Champion

# Owner's Responsibilities

## Track issues

- Create, triage and track issues or new features with github issue id
- Orgnize github issues ids in project tab with tech area and assignee shown

## Review commits

- Create a pull request to review any document change/commit
- Specify reviewers both in vendor side and FP side in that pull request
- Review commits in pull requests on timingly basis (2 days deadline)
  by pushing review button

## Maintain Deliverables

- Maintain good file structure in folder by following file and folder
  name conventions# Table of Contents

- [QA Workflow](#qa)
- [Development Workflow](#dev)
- [Change Management](#chg)
- [Design Package](#pkg)

# Execution

## Stages

1. Draft Definition
2. Project Champion(Business Owner)Review
3. Team member review 
4. Finalize and release workflow
5. Team members excute the released procedure

## Execution Feedback
- Comments on non-compliance
- Correction within 2 days following released standard
- New issues may be created for continious improvements

## Escalation
1. Facts collection
2. Refine definition
3. Management involvement
4. Suspending account in github if non-compliance can not be resolved within 7 days
5. Suspending project and archive repo if status cannot be maintained


# QA Workflow <a id="qa"></a>

Define status with time line and accountable assignee to track bugs or defects effectively during production stage.

- [QA Status](#qa-status)
- [Github Project Fields](#gh-field)

## QA Status <a id="qa-status"></a>
1. [Open](#qa-open)
2. [Triage](#qa-triage)
3. [Root Cause Analysis (RCA)](#qa-rca)
4. [Fix](#qa-fix)
5. [Done](#qa-done)

### Open <a id="qa-open"></a>
- Assignee: issue reporter
- Time block: 1 week
- Key information: 
  - Product Code
  - S/N
  - Precise bug or defect symptom
  - Tracking Number 

### Triage <a id="qa-triage"></a>
- Assignee: vendor QA lead
- Time block: 10 days
- Determine:
  - Assignee
  - Priority
  - Duplicates

### RCA <a id="qa-rca"></a>
- Assignee: vendor engineer
- Time block: depending on priority
- Key deliverables:
  - Vendor defect reports, or
  - Manufacture reports

### Fix <a id="qa-fix"></a>
- Assignee: vendor engineer
- Key deliverables:
  - Design changes, or
  - SOP changes
  - Pull request
  - Supporting documentation

### Done <a id="qa-done"></a>
- Assignee: issue reporter
- It's issue reporter's decision to close or not.

## Github Project Fields <a id="gh-field"></a>

- [Assignee](#gh-assignee)
- [Status](#gh-status)
- [Duplicate](#gh-duplicate)
- [Label](#gh-label)
- [Dates](#gh-date)

### Assignee <a id="gh-assignee"></a>
- A single person who is responsible for the current status

### Status <a id="gh-status"></a>
- A single select field to indicate status

### Duplicate <a id="gh-duplicate"></a>

- A text field to indicate this issue is a duplicate of another same issue. 
- Product Code: Issue ID

### Label <a id="gh-label"></a>

- A multi-select text field to indicate what are deliverables for this task or issue
- A report must be labelled when in RCA 
- Label can be used for many different purpose as long as definitions in one project are consistent 

### Open, RCA Start and Fix Date <a id="gh-date"></a>

- Date format fields to tracking time and status
- These field can also be used to generate meaningful performance indicator through filters, e.g. Q1 Open, Q2 Fix, etc. 


# Development Workflow <a id="dev"></a>

To be able to divide and conquer and track incremental changes during development stage

- [Task](#dev-task)
- [Trackor](#dev-trackor)
- [Assignee](#dev-assignee)
- [Priorities](#dev-priorities)
- [Status](#dev-status)
- [Area](#dev-area)
- [Deliverable](#dev-deliverable)
- [Timelines](#dev-timelines)

## Task <a id="dev-task"></a>

A single action item, e.g.

- Feature Request
- Bug Reports
- Test Case

A task may have a todo checklist.

## Trackor <a id="dev-trackor"></a>

A group of action items or sub trackors, e.g.

- Situation Appraisals
- Release Notes
- Test Plans

The rule of divide-and-conquer:
- A trackor must have a list of tasks or smaller trackors
- A trackor or a task must have deliverables defined or lablled

## Assignee <a id="dev-assignee"></a>

Each task or trackor must have a single person as assignee.

## Priorities <a id="dev-priorities"></a>

A ranking of importance and urgency

- High
- Medium
- Low

## Status <a id="dev-status"></a>

Indicate what is the current stage of a specific trackor or task

1. Open
2. Triage
3. Progess
4. Review
5. Done
6. Backlog

## Area <a id="dev-area"></a>

Functional domain of trackors or tasks,e.g
- PRODUCT
- ID
- SW
- HW
- MEC
- TEST
- QA
- PRODUCTION
- MARKETING

## Deliverable <a id="dev-deliverable"></a>

Results of tasks or trackors. All deliverables are certain format of documents, e.g.
- bin: s/w release binaries
- howto: tutorials
- id
- sw: s/w source code
- scripts
- sch: schematic
- pcb
- bom
- bom:cost
- mec
- test:plan
- test:rst 
- test:tc
- doc: prd, mkt

## Timelines <a id="dev-timelines"></a>

Short term and long term goals,

- Roadmap
- Milestone
- Sprint
- Start date and target date

## Risk <a id="dev-risk"></a>

Risk should be assessed on a trackor or task with timeline, especially a critical path. And it should be regularly updated.

- On Track
- At Risk
- Blocked

# Change Management <a id="chg"></a>

## General Guideline

Changes should be managed in an increasingly, more and more restrictive manner with more milestone achieved.

- Initially duing development, it serves more of a personal tracking tool for developers to exploring ideas and easily going back when ideas fail.
- After prototypes work, it serves more of building tool for developers to keeping building more things without breaking existing or impacting others.
- During preproduction or production stage, changes must be managed strictly to ensure solving problems not creating new problems or disastors.

- [ ] commit message
- [ ] branch
- [ ] reviews

## Design Package <a id="pkg"></a>

- [ ] folders
- [ ] releases


# Github Howtos and Admin

## Project Board <a id="howto-project"> </a>

- [Docs](https://docs.github.com/en/issues/trying-out-the-new-projects-experience/quickstart)
- Navigation
- Field
- Views
- Filters

## Markdown <a id="howto-md"></a>

# Folder Structure and Ownership


# Owner's Responsibilities

## Track issues

- Create, triage and track issues or new features with github issue id
- Orgnize github issues ids in project tab with tech area and assignee shown

## Review commits

- Create a pull request to review any document change/commit
- Specify reviewers both in vendor side and FP side in that pull request
- Review commits in pull requests on timingly basis (2 days deadline)
  by pushing review button

## Maintain Deliverables

- Maintain good file structure in folder by following file and folder
  name conventions

docstructure.
--->
## Guidelines

There are many factors to consider where to put documents in github,
below are 3 fundamental principles

- Ownership
- Type of documents: text, binary, code
- Type of developments: product, firmware, javascript, python, etc.

??? Info "todo"

    I will setup a discussion and standardize the most common use case
    for our product development use case with domain engineers and
    vendor teams.

## Binaries

Folder | Description
-- | --
bin/ | software binaries 
bom/ | Build of Materials 
cert/ | Compliance certificates
datasheet/ | Component datasheets
docs/ | Mardown documents
flow/ | Flowchart
gfx/ | On-product graphics
mec/ | Assemblies and custom parts
pcb/ | PCB design files 
print/ | packaging and inserts
qa/ | Quality assurance data
sch/ | Schematic design files
sop/ | Standard Operation Procedures
test/ | Test data
