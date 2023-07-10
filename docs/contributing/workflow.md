# Document workflow

## How to solve a problem?

Below is a common sense.

```mermaid
flowchart TD
  A([Understand Problems])
  B([Define Problems])
  C([Find Root Causes or Options])
  D([Provide Solutions])
  E([Verify Solutions])
  A-->B
  B-->C
  C-->D
  D-->E
```

But too many times, people just do shortcuts,

```mermaid
flowchart TD
  A([Take Problems])
  E([Jump into Solutions])
  A-->E
```

If people take wrong problems and jump right into solutions, usually
it ends up with a much bigger problem.

## Basic Documentaion Flow in Github

```mermaid
flowchart TD;
  A([Understand Problems in Github Discussions])
  B([Define Problems with Markdowns])
  C([Find Root Causes or Options with Issue Updates])
  D([Provide Solutions through Commits and Pull Requests])
  E([Verify Solutions with Markdown and Commits])
  A-->B
  B-->C
  C-->D
  D-->E
```

All problems or ideas shoud start in a team-based Github discussion
area where all histories can be retained and topics can be categoried.

As long as the problems or idea is fully understand, it should go into
repo by transfering Discussion topics to repo issues, or create new
issues.

Our first goal here is to prove problems themselves and it is not to
provide solutions. We don't have this well-defined today. Here we need
version-controlled requirements.

Our second goal is to prove root causes and evaluate all options. Here
again it is not to provide solutions. Here we need version-controlled
tests and data. And provides better comment updates on root cause
analysis.

Once we understand root causes and evaluate possible options the best
solution speak itself. Changes in all areas must be identified and
tracked. 

Once we understand all changes in all areas, we can decide the scope
of project with ownership and deliverables defined.

## Example Document Flow

```mermaid
flowchart TD;
  subgraph A[Understanding problems or ideas in Github Discussions]
  A1([Returns])
  A4([Market Research])
  A5([Sales emails])
  A6([New ideas])  
  Aout([Validate Problems or Ideas])
  A1-->Aout
  A5-->Aout
  A4-->Aout
  A6-->Aout
  end

  subgraph B[Definitions - Feature Requests]
  B1([Customer Requirements])
  B2([Technical Requirements])
  Bout([Prove problems])
  B1-->Bout
  B2-->Bout
  end

  subgraph C[Scoping - Test Cases]
  C1([RCA])
  C2([Options])
  Cout([Prove root causes or Evaluate all options])
  C1-->Cout
  C2-->Cout
  end

  subgraph D[Commits]
  D1([Customer Requirements])
  D2([Technical Requirements])
  D1-->D2
  end

  D2-->E{Released?}
  E-->|Yes| F[Project Committed]
  E-->|No| G[Further Validate and Prove Problems]

  A-->B-->C-->D
```

## Basic Guidelines

- Don't using emails to develop projects. Put everything in discussion
  area for a product/project if not sure;

- Update facts, data, logs or whatever new findings in a github issue which is
  a single source of truth. Don't only update status in the issue;

- Plan projects in discussion area. Don't plan that in github
  issues. The plan itself is not a deliverable and not source of
  truth;

- Use issue top comment box to preview the document changes you are proposing;

## Document Workflow in Github

??? Warning "Compliance"

    2 things are mandatory or required for compliance. One is all
    product ideas or tech topics must be registered in general
    discussions pending validation.One is all tech docs will be
    written by Markdown lauguage.

### Discussions

Any topic including ideas, suggestions, support requests, project
status and planning, technical Q&A, show off, release announcements,
etc., anythiny should be first registered in discussion.

This is to replace email traffic and increase visibility, so the whole
community knows what is going on, project participants can provide
early feedbacks, and deliverable owners have opportunities do more
upfront evaluations before actually committing into an ongoing
projects.

- Each vendor has only one discussion area;
- Topics are categoried in predefined categories;
- Topics are further grouped by labels or tags;
- No owner and change management requirements
- Any discussion is not in a project scope

### Issues

Github Issues are used to develop features and test cases, improve
designs, report bugs, validate problems, break down works, etc.,
facilitate teamwork, communications and reviews.

However, contents in issue thread don't have change management and
they cannot replace version controlled deliverables. We will regulate
issue usage in the following ways,

- Each issue has a single owner or assignee who owns or produce version controlled document;
- Each issue has a single target or deliverable, it cannot represent different deliverables;
- If one issue has multiple assignees or deliverables, specific issues must be created;
- Issue content in top box can be used to track document changes or used as copy-paste for markdown commits;
- Issue content in comment box must be addressed with "hide" options

### Docs and Binaries

We address issues by making changes to existing documents. In general,
changes in id designs, mechanical drawings, schematics, pcb, bom, bin,
datasheets, test data etc. are binaries, software changes are in its
own categary, and all other changes, e.g. requirements, designs,
reports, test cases are text based.

All docs (non binary or software) must be maintained in a docs folder.

Below is an ESD example, each block has github issue with one owner and
end docs defined.

```mermaid
---
title: ESD Example
---
classDiagram
    CRD --|> TRD
    CRD --|> TC1
    CRD --|> TC2
    TC1 --|> Acceptance
    TC2 --|> Acceptance
    TRD --|> CRD
    TC --|> Release
    TC --|> TRD
    TC --|> Test
    TC <|-- TRD
    Bug <|-- Test
    PCB <|-- Bug
    SCH <|-- Bug
    BOM <|-- Bug
    Bug --|> MEC
    MEC --|> SOP

    class CRD {
        ESD pressure shocks
        FR: ESD charging systems
        docs/crd.md
    }

    class TRD {
        ESD 8kV requirements
        FR: ESD 8kV
        docs/trd.md
    }

    class TC {
        ESD test cases
        + TC: ESD 8kV + 16kV
        docs/tests/esd.md
    }

    class Bug {
        ESD test fails
        + BR: ESD
        docs/design/esd-root-cause.md
        docs/tests/esd.md
    }

    class Test {
        ESD test data
        TC: ESD
        ./test/esd.exel
    }

    class PCB{
        PCB
        FR: PCB changes for ESD 
        pcb/product.pcb
    }

    class SCH{
        SCH
        FR: SCH changes for ESD 
        sch/product.sch
    }

    class BOM{
        BOM
        FR: BOM changes for ESD 
        bom/bom.exel
    }

    class MEC{
        MEC
        FR: Hook changes for ESD
        FR: Add conduction for ESD
        mec/product.mec
    }

    class SOP{
        SOP
        FR: SOP changes for ESD
        docs/sop/esd.md
    }

    class Release {
        Product Release Test Plan
        RN: 1.0
        docs/testplan/prototype.md
        docs/testplan/release.md
    }

    class Acceptance {
        FP Acceptance Test Plan
        RN: 1.1
        docs/testplan/acceptance.md
    }

    class TC1 {
        ESD tank shock 
        + TC: ESD refrigerant shot
        docs/tests/esd-tank.md
    }

    class TC2 {
        ESD Field or Beta Tests
        + TC: Hook on condensor
        docs/tests/esd-fields.md
    }

```