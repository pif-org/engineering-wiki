# Development lifecycle

<aside>
💡 This page documents the development process engineers should follow. Helpful for getting up to speed when joining the team.

</aside>
<br>

<aside>
**We don't use rebase!** to disable it, run this
</aside>

```bash
git config --global pull.rebase false
```

# 1. Create a branch off of `develop`

Name the branch with your first name pre-pended:
`leslie/cool-feature`

# 2. Writing code

Implement the new feature, bug fix, doc or enhancement and ensure
- Your new change doesn't break anything
- Write a Unit, Integration or End to End test when necessary
- Ensure you fix all linting, typescript and prettier issues
- Pull from develop again and ensure you fix any merge conflict
- Finally, push your feature branch

## Commit messages

Make sure your commit messages are descriptive. Make sure you follow [conventional commit guidelines](https://www.conventionalcommits.org/en/v1.0.0/)

# 3. Create a pull request on Github

Include the Github Project task link in your PR description e.g `[Task name](https://github.com/orgs/pif-org/projects/2/views/1?pane=issue&itemId=25000166)`

# 4. Submit for review

- Assign the task in Notion to the appropriate reviewer.
- You can always tag a person on a Notion page by typing `@` followed by their name.

<br>

# ✔️ Performing code reviews

### How to review

- Make two passes over the PR if it's substantial.
    - On the first pass, come to an understanding of the code change at a high level.
    - On the second pass, pay more attention to semantic details.

# Examples

```jsx
var commentCount = 0;
```

You might suggest that this be a `let` instead of `var`.