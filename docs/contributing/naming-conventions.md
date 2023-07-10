# Naming Conventions

## Github Account ID naming convention

The github id is **lower case** with a company id and your email id
connected with a hyphen in between.

Your **full name** MUST be in public profile. For more information,
see [Howtos](../../github/howtos)


`<company id>-<email id>`

??? Info "For example"
    `fp-hyang`

??? Warning "Full email"

    Any member or collaborator must be fully identified. Currently
    there is no requirement to ask full email id
    (username@company.com) in public profile. That exposure increases
    risks of spam.

    So, your account id is the most important way for team members to
    quickly and easily identify who you are and what company you work
    for and for admin to assign you to proper github teams.  Through
    "teams", permissions, data securities and vendor isolation are
    managed.

??? Warning "Leaving"

    When people leave organizations including both Fieldpiece and
    vendors or when people no longer work on projects, it is site
    owner's responsibility to remove them on timingly manner. A well
    defined project team will help this.
    
## Github Repo Naming Convention <a id="repo-naming"></a>

All repo names in Fieldpiece github consist of 3 IDs,

```text
<company id>-<product id>-<content id>
```

### Company ID

Fieldpiece owns all documents in all repos. Vendor ID helps identify
the visibility of that repo.

### Product ID

Prefer one major product has one repo. All other Fieldpiece
confidential or internal can be hosted in one repo through folder and
project structures.

### Content ID

Content ID helps describe what repo content could be. "doc" means almost
everything, id designs, mec, electronics, tests, qa, etc.  "fw" or
"sw" means product software source code. If code base is not big
enough, the software source code could be just in a "doc" subfolder.

## Folder Naming Conventions

A folder can be viewed as a funtional module of a document
system. Well-structured folders help identify ownership and track
changes(more on this in "commit message guidelines")

- Use lower cases
- Connect words by underscores "_"
- Don't leave space between words
- Try to use meaningful simplifications, e.g. people know "pcb", but
  may not know "fc" (flowchart)

??? Info "Predefined"

    Folder name | Description
    -- | --
    bin/ | binary releases
    bom/ | build of materials
    cert/ | product certificates
    mec/ | mechanical
    pcb/ | PCB 
    pkg/ | box, manual, forms etc
    docs / | document source
    sch/ | schematic
    sop/ | standard operations
    test/ | test cases, plans and results
    qa/ | quality assurance

    More to come.

## File Naming Conventions

A concise and consistent file naming help idtenfy contents and reduce
folder structure depth.

- Use hyphen "-" to connect well spelled and meaningful English words
- "folder-and-file-naming-conventions.md"
- "README.md" This is the readme filename for all folders.

## Project Naming Conventions

- Use capital cases
- Vendor id and project code with space in between

??? Info "For example"

    FP ROCKETII


## Branch Naming Conventions

Branch naming can be flexible since most branches are short-living for
a bug fix, test data, or feature development.

- Use lower cases
- Connect words by hyphen "-"

??? Info "For example"
    ```
    fr-123
    tc-data-456
    ```

However when a long-live bracnch is required, e.g. github default
branch is "main" changed from "master" and github pages default branch
is "gh-pages", we have to reduce randomness of naming. Think the
branch as a totally different view of data or files in a same
repo, naming can be a big decision making. We could start sman6
with a new branch called 'dev', rather creating a new repo, for
example.

<!--

Purpose to use github
- Visibility
- Concise and precise communication
- Divide-and-conquer of deliverables
- Project management from tech aspect

Deliverables - development/production package
- repos and orgs
- folder structure
- template repo
- naming conventions
- basic workflows

Issues and issue template
- Feature request
- Bug report
- Test case
- Situation appraisal
- Release

Commits
- Commit messages
- View histories

Pull Requests
- Branches
- Reviews and merges

-->