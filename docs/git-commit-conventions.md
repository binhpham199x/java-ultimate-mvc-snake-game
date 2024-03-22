# Conventional Commit Messages
See how a [minor change](#examples) to your commit message style can make a difference.

## Commit Message Formats
### Default
<pre>
<b><a href="#types">&lt;type&gt;</a></b></font>(<b><a href="#scopes">&lt;optional scope&gt;</a></b>): <b><a href="#description">&lt;description&gt;</a></b>
<sub>empty separator line</sub>
<b><a href="#body">&lt;optional body&gt;</a></b>
</pre>



### Inital Commit
```
init
```

### Types
* Relevant changes
    * `feat`  Commits, that adds or remove a new feature
    * `fix`   Commits, that fixes a bug
* `refactor`  Commits, that rewrite/restructure your code, however does not change any API behaviour
    * `perf`  Commits are special `refactor` commits, that improve performance
* `style`     Commits, that do not affect the meaning (white-space, formatting, missing semi-colons, etc)
* `test`      Commits, that add missing tests or correcting existing tests
* `docs`      Commits, that affect documentation only
* `build`     Commits, that affect build components like build tool, ci pipeline, dependencies, project version, ...
* `ops`       Commits, that affect operational components like infrastructure, deployment, backup, recovery, ...
* `chore`     Miscellaneous commits e.g. modifying `.gitignore`

### Scopes
The `scope` provides additional contextual information.
* Is an **optional** part of the format
* Allowed Scopes depends on the specific project
* Don't use issue identifiers as scopes

### Body
The `body` should include the motivation for the change and contrast this with previous behavior.
* Is an **optional** part of the format
* Use the imperative, present tense: "change" not "changed" nor "changes"
* This is the place to mention issue identifiers and their relations


### Description
The `description` contains a concise description of the change.
* Is a **mandatory** part of the format
* Use the imperative, present tense: "change" not "changed" nor "changes"
    * Think of `This commit will...` or `This commit should...`
* Don't capitalize the first letter
* No dot (`.`) at the end

### Examples
* ```
  feat: add email notifications on new direct messages
  ```
* ```
  feat(shopping cart): add the amazing button
  ```

* ```
  fix(api): handle empty message in request body
  ```
* ```
  fix(api): fix wrong calculation of request body checksum
  ```
* ```
  fix: add missing parameter to service call

  The error occurred because of <reasons>.
  ```
* ```
  perf: decrease memory footprint for determine uniqe visitors by using HyperLogLog
  ```
* ```
  build: update dependencies
  ```
* ```
  build(release): `bump version to 1.0.0
  ```
* ```
  refactor: implement fibonacci number calculation as recursion
  ```
* ```
  style: remove empty line
  ```


## References
* https://gist.github.com/qoomon/5dfcdf8eec66a051ecd85625518cfd13
* https://www.conventionalcommits.org/en/v1.0.0/#summary