# Writing on GitHub

## Start writing on GitHub

### Quickstart
<details>
<summary>My top languages</summary>

| Rank | Languages  |
| ---: | ---------- |
|    1 | JavaScript |
|    2 | Python     |
|    3 | SQL        |

</details>

---
> If we pull together and commit ourselves, then we can push through anything.

— Mona the Octocat

### [Basic writing and formatting syntax](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)

#### Footnotes

```markdown
Here is a simple footnote[^1].

A footnote can also have multiple lines[^2].

[^1]: My reference.
[^2]: To add line breaks within a footnote, prefix new lines with 2 spaces.
  This is a second line.
```

Here is a simple footnote[^1].

A footnote can also have multiple lines[^2].

[^1]: My reference.
[^2]: To add line breaks within a footnote, prefix new lines with 2 spaces.
  This is a second line.

#### Alerts
```markdown
> [!NOTE]
> Useful information that users should know, even when skimming content.

> [!TIP]
> Helpful advice for doing things better or more easily.

> [!IMPORTANT]
> Key information users need to know to achieve their goal.

> [!WARNING]
> Urgent info that needs immediate user attention to avoid problems.

> [!CAUTION]
> Advises about risks or negative outcomes of certain actions.
```

> [!NOTE]
> Useful information that users should know, even when skimming content.

> [!TIP]
> Helpful advice for doing things better or more easily.

> [!IMPORTANT]
> Key information users need to know to achieve their goal.

> [!WARNING]
> Urgent info that needs immediate user attention to avoid problems.

> [!CAUTION]
> Advises about risks or negative outcomes of certain actions.


## Work with advanced formatting
### Organized data with tables
You can align text to the left, right, or center of a column by including colons : to the left, right, or on both sides of the hyphens within the header row.


```markdown
| Left-aligned | Center-aligned | Right-aligned |
| :----------- | :------------: | ------------: |
| git status   |   git status   |    git status |
| git diff     |    git diff    |      git diff |
```

| Left-aligned | Center-aligned | Right-aligned |
| :----------- | :------------: | ------------: |
| git status   |   git status   |    git status |
| git diff     |    git diff    |      git diff |

### Collapsed sections

````markdown
<details>

<summary>Tips for collapsed sections</summary>

### You can add a header

You can add text within a collapsed section. 

You can add an image or a code block, too.

```ruby
   puts "Hello World"
```

</details>
````

<details>

<summary>Tips for collapsed sections</summary>

### You can add a header

You can add text within a collapsed section. 

You can add an image or a code block, too.

```ruby
   puts "Hello World"
```

</details>

### Create code blocks
To display triple backticks in a fenced code block, wrap them inside quadruple backticks.

````
```
Look! You can see my backticks.
```
````


### [Create diagrams](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/creating-diagrams)

Check it later.


### [Mathematical expressions](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)

[The MathJax website](http://mathjax.org/)

### Auto linked references
References to URLs, issues, pull requests, and commits are automatically shortened and converted into links.


### Attaching files


### About task lists
You can use task lists to break the work for an issue or pull request into smaller tasks, then track the full set of work to completion.

```
- [x] #739
- [ ] https://github.com/octo-org/octo-repo/issues/740
- [ ] Add delight to the experience when all tasks are complete :tada:
```

- [x] #739
- [ ] https://github.com/octo-org/octo-repo/issues/740
- [ ] Add delight to the experience when all tasks are complete :tada:

### [Permanent links to code](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/creating-a-permanent-link-to-a-code-snippet)
You can create a permanent link to a specific line or range of lines of code in a specific version of a file or pull request.

Check it later.


### Using keywords in issues and pull requests
Use keywords to link an issue and pull request or to mark an issue or pull request as a duplicate.


## Work with saved replies
### About saved replies
You can use a saved reply to respond to an issue or pull request.

暂时用不到。


## Share content with gists

### Creating gits

You can create two kinds of gists: public and secret. Create a public gist if you're ready to share your ideas with the world or a secret gist if you're not.


### Forking and cloning gists
Gists are actually Git repositories, which means that you can fork or clone any gist, even if you aren't the original author. You can also view a gist's full commit history, including diffs.

