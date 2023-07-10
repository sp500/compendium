# Search and Filter

Think everything on github is a giant excel table, you do need to filter out information quickly.

## Understanding GitHub's Search Bar

### Location of the Search Bar

The search bar is conveniently located at the top of any page on
GitHub. Whether you're on your profile page, browsing a repository,
looking at issues, or just on the GitHub homepage, the search bar is
always there.

### How to Reach the Search Bar Quickly

In most web browsers, you can quickly jump to the search bar by
pressing the '/' key on your keyboard, no matter where you are on the
page. You just press '/' and start typing your query. This is a handy
shortcut to keep in mind, as it saves you the trouble of scrolling
back to the top of the page or reaching for your mouse.

### Using the Search Bar

Once you're in the search bar, you can start typing your query. As you
type, GitHub will display a dropdown with relevant suggestions
including repositories, users, or issues that match your query. You
can use your keyboard's arrow keys to navigate through these
suggestions and press 'Enter' to select one.


### Selecting the Scope of the Search

You can click the dropdown of the search bar to choose where you want
to search. The options include 'In this repository', 'In this user',
and 'In all of GitHub'. By default, 'In all of GitHub' is selected,
which means your search will return results from all public
repositories.


### Keywords, Phrases, and Qualifiers

You can type keywords, phrases, or specific search qualifiers in this
bar.

**Keywords**: These are individual words that you enter into the
search bar to find relevant content. When you search with keywords,
the search engine will return results that contain all of these words,
but not necessarily in the order you typed them. For example, if you
enter the keywords **neural network**, GitHub's search engine will
return all repositories that contain both **neural** and **network**
anywhere in their content.

**Phrases**: If you want to search for a specific combination of words
in the exact order, you should use a phrase search. To do this, you
simply put your search terms in quotation marks. For example, if you
search **"neural network"**, GitHub's search engine will only return
repositories that contain the exact phrase **neural network**.

**Qualifiers**: Qualifiers are special instructions that you can
include in your search to make it more precise. On GitHub, you can use
qualifiers to specify where to search for your keywords or phrase,
filter results based on certain criteria, and more. For example, the
qualifier **in**:name instructs GitHub to look for your keywords or
phrase only in repository names.

Here are a few other examples of GitHub's search qualifiers:

**is:** Filters the search based on the state of issues or pull
requests (e.g., is:open or is:closed).

**user:** or **org:**: Restricts the search to repositories owned by a
specific user or organization.

You can use these qualifiers individually or in combination to refine
your search. For example, language:python stars:>100 would find Python
repositories with more than 100 stars.

## Advanced Search

### Quick Access to Github Advanced Search

In GitHub, you can quickly access the advanced search from any page by
using the search bar at the top of the screen:

1. Click in the search bar or press '/' on your keyboard to focus on it.
2. Without typing anything into the search bar, press 'Enter'. This will
take you to the advanced search page.


### Using Advanced Search

The Advanced Search page on GitHub provides a more structured
interface for performing complex searches. Here's how you can use it:

**Search Term**: At the top of the Advanced Search page, there's a box
  for your search terms. This works just like the regular search bar:
  you can type in keywords, phrases (in quotation marks), and even use
  qualifiers.

**Search Qualifiers**: Below the search term box, there are several
  sections that allow you to add qualifiers to your search without
  having to remember the syntax.

For example, in the "Repositories options" section, you can specify
the number of stars or forks a repository has, or the language it's
written in. In the "Issue/Pull request options" section, you can
filter by the issue or pull request's state, associated labels, and
more.

**Issues and Pull Requests Search**: You can search within issues and
  pull requests content by choosing the "Issues" or "Pull requests"
  options beside the search box. This can be very helpful when trying
  to find certain discussions or decisions made in a project.

**Users and Organizations Search**: If you want to find a specific
  user or organization, select the "Users" or "Organizations" option
  and enter the name.

Once you've filled in your search criteria, click the 'Search' button
at the bottom of the page (or just press 'Enter') to perform your
search. Your search results will be displayed in a new page, where you
can further sort and filter them if needed.

Remember, the more specific your search criteria, the more accurate
your search results will be. Don't be afraid to use multiple
qualifiers to narrow down your search.

## Qualifiers

### Issue and Pull Request Search Qualifiers

Matches issues or pull requests based on their state:

```
is:open
is:closed
is:merged
is:unmerged
is:draft
is:pr
is:issue
```

Matches issues or pull requests based on the involvement of a user or team:

```
author:USERNAME
assignee:USERNAME
mentions:USERNAME
commenter:USERNAME
involves:USERNAME
team:TEAMNAME
```

Limits searches to a specific repository or organization.

```
repo:USERNAME/REPO
org:ORGNAME
```


Matches issues linked to pull requests and vice versa:

```
linked:pr or linked:issue
```

Matches issues or pull requests based on dates:

```
created:YYYY-MM-DD
updated:YYYY-MM-DD
merged:YYYY-MM-DD
closed:YYYY-MM-DD
```

Matches issues or pull requests based on the number of comments:

```
comments:n
```

Matches issues or pull requests based on the number of interactions:

```
interactions:n:
```

Matches issues or pull requests based on the number of reactions:
```
reactions:n: 
```

### Repository Search Qualifiers

Matches repositories owned by a certain organization.

```
org:Fieldpiece
```

Search in the name, description, and readme respectively:

```
in:name
in:description
in:readme
```

Matches repositories with these topics

```
topics:TOPIC1,TOPIC2
```

Other qualifiers:

```
size:n: Matches repositories that are n kilobytes in size.
forks:n: Matches repositories with n forks.
stars:n: Matches repositories with n stars.
created:YYYY-MM-DD: Matches repositories that were created by a certain date.
pushed:YYYY-MM-DD: Matches repositories that were pushed to by a certain date.
language:LANGUAGE: Matches repositories written in a certain language.
is:public or is:private: Matches public or private repositories.
archived:true or archived:false: Matches archived or non-archived repositories.
mirror:true or mirror:false: Matches mirrored repositories.
```

### Combining Qualifiers

You can combine multiple qualifiers to make your search even more
specific. Just separate each qualifier:term pair with a space. For
example, **language:javascript stars:>1000 in:name** would find
JavaScript repositories with more than 1000 stars and your keyword in
their name.

## Links

### Several quick start links

- [Search on Gihub](https://docs.github.com/en/search-github)
- [Search Syntax](https://docs.github.com/en/search-github/getting-started-with-searching-on-github/understanding-the-search-syntax)
- [Search Issues and PRs](https://docs.github.com/en/search-github/searching-on-github/searching-issues-and-pull-requests)
- [Filtering projects](https://docs.github.com/en/issues/planning-and-tracking-with-projects/customizing-views-in-your-project/filtering-projects)
