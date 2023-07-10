## Format

> primary:secondary: subject text [<- this is subject line]
>
> body text
>
> _issue_: Github Issue ID
>
> Signed off footer (optional)

??? Info "Example 1"
    ```
    sch: replace schottky diode SS14 with 4007

    The reverse bias voltage of 4007 is higher than ss14. This higher
    reverse bias prevents wrong detection of USB cable.

    Issue: https://github.com/Fieldpiece/xxx/issues/243
    ```

??? Info "Example 2"
    ```
    pt: change R-452b static code to 49

    R428A and R452B share the same static code, and one of them has to
    change.

    Issue: #471
    ```

## Subject Line Rules

- Primary and/or secondary are the primary and/or secondary modules
  you are working on. They are folder names in most cases.

- The subject line briefly describe only what INCREMENTAL CHANGE is

- The INCREMENTAL CHANGE is defined as the more information relative
to the previous commit

- Use the imperative mood in the subject line

- The total number of characters in subject line is less than 72
characters

- Do not end the subject line with a period

## Text Body Rules

- Each commit MUST be linked to an issue id

- Separate subject from text body with a blank line

- Text body may provide more change details or summary. In most cases,
  you can leave out details about how a change has been made

- Text body explains in high level why the change is needed.

- Capitalize each paragraph in text body

- Wrap lines at 72 characters

- Each commit should address a single feature or bug

- Use present tense, not past tense

## Why do we need a good commit message?

- This is the first step to show how a good development, communication
  and clear thinking happen.

- By providing a good subject line to describe the CHAGNGE concisely
  you think better what you are doing and you can communicate better
  what you did.

- By providing reasons for changes in body text you know better why
  you are doing stuff.

- Issue ID MUST be attached to a commit message body. NO EXCEPTION!
  Information tracked in issue discussion provides much greater
  context of why stuff is needed.
 