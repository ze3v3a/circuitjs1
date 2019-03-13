## Welcome Contributor! :heart: 

This is the contributor page for the Browser based Circuit Simulator project `circuitJS1`.

We are dearly excited that you are interested in contributing to this project. However,
it is very importtant to try to adhere to some standards regarding the coding style. 
This is your guide for doing so. The following text is meant as a guideline, but in 
reality you can probably skip most of the text below.

#### Our Coding Style 

Here is a list of a few things we require to conform to our coding style:

* Please use a `4-space` tabulator stop and do not use `TAB` characters for code formatting.  
  (I actually love TABs, but most people don't know how to use different spacings.)
* Do not remove my code comments, unless they are wrong. I love keeping sensible comments!
* Do not use that \*effin' Java commenting style with bunch of `/** usless blah */`.
* Keep the MAX code line lengths between 100-140 characters, before wrapping.  
  (If you are not able to tune you GUI or screen to use full length, you probably shouldn't be coding!) 
* Use `function() {` rather than `function (){`.
* Avoid using a separate line for the **starting** curly bracket, `{`, unless its in a JSON or object.  
* Use **UTF-8** file encoding where possible
* **IMPORTANT:** :exclamation: `End all files with a newline!` :exclamation: 


I think that's about it, for now.

Thanks again for wanting to contribute!

:heart: 

**END**

---

#### How Do I Submit A (Good) Bug Report?

Bugs are tracked as [GitHub issues](https://guides.github.com/features/issues/). 
Create an issue on this repository and provide the following information by 
filling in [the template](ISSUE_TEMPLATE.md).

Explain the problem and include additional details to help maintainers reproduce the problem:

* **Use a clear and descriptive title** for the issue to identify the problem.
* **Describe the exact steps which reproduce the problem** with as many details as possible.
* **Provide specific examples to demonstrate the steps**. Include links to files or GitHub projects, or copy/pasteable snippets, which you use in those examples. 
* **Describe the behavior you observed after following the steps** and point out what exactly is the problem with that behavior.
* **Explain which behavior you expected to see instead and why.**
* **Include screenshots and/or animated GIFs** which clearly demonstrate the problem. 
* Include details about your configuration and environment:


### Pull Requests

* Fill in [the required template](PULL_REQUEST_TEMPLATE.md)
* Do not include issue numbers in the PR title
* Follow the [JavaScript](#javascript-styleguide) and [CoffeeScript](#coffeescript-styleguide) styleguides.
* Document new code based on the [Documentation Styleguide](#documentation-styleguide)

---

## Styleguides

### Git Commit Messages

* Use the present tense ("Add feature" not "Added feature")
* Use the imperative mood ("Move cursor to..." not "Moves cursor to...")
* Limit the *first* line to 72 characters or less
* Reference issues and pull requests liberally after the first line
* When only changing documentation, include `[ci skip]` in the commit title
* Consider starting the commit message with an applicable emoji:
    * :art: `:art:` when improving the format/structure of the code
    * :racehorse: `:racehorse:` when improving performance
    * :memo: `:memo:` when writing docs
    * :bug: `:bug:` when fixing a bug
    * :fire: `:fire:` when removing code or files
    * :green_heart: `:green_heart:` when fixing the CI build
    * :white_check_mark: `:white_check_mark:` when adding tests
    * :lock: `:lock:` when dealing with security
    * :arrow_up: `:arrow_up:` when upgrading dependencies
    * :arrow_down: `:arrow_down:` when downgrading dependencies


### JavaScript Styleguide

All JavaScript must adhere to [JavaScript Standard Style](https://standardjs.com/).

* Prefer the object spread operator (`{...anotherObj}`) to `Object.assign()`
* Inline `export`s with expressions whenever possible
  ```js
  // Use this:
  export default class ClassName {

  }

  // Instead of:
  class ClassName {

  }
  export default ClassName
  ```

### CoffeeScript Styleguide

* Set parameter defaults without spaces around the equal sign
    * `clear = (count=1) ->` instead of `clear = (count = 1) ->`
* Use spaces around operators
    * `count + 1` instead of `count+1`
* Use spaces after commas (unless separated by newlines)
* Use parentheses if it improves code clarity.
* Prefer alphabetic keywords to symbolic keywords:
    * `a is b` instead of `a == b`
* Avoid spaces inside the curly-braces of hash literals:
    * `{a: 1, b: 2}` instead of `{ a: 1, b: 2 }`
* Include a single line of whitespace between methods.
* Capitalize initialisms and acronyms in names, except for the first word, which
  should be lower-case:
  * `getURI` instead of `getUri`
  * `uriToOpen` instead of `URIToOpen`
* Use `slice()` to copy an array
* Add an explicit `return` when your function ends with a `for`/`while` loop and
  you don't want it to return a collected array.
* Use `this` instead of a standalone `@`
  * `return this` instead of `return @`

---

### Issue and Pull Request Labels

This section lists the labels we use to help us track and manage issues and pull requests (PR's). 

#### Type of Issue and Issue State

| Label name | Description |
| --- | --- |
| `enhancement` | Improvments and *New* Feature requests |
| `bug`         | Confirmed bugs or reports that are very likely to be bugs |
| `question`    | Questions more than bug reports or feature requests (e.g. how do I do X) |
| `feedback`    | General feedback more than bug reports or feature requests |
| `help-wanted` | Request help from the community in resolving the issue |
| `good-first-issue`        | Less complex issues which would be good first issues to work on |
| `more-information-needed` | More information needs to be collected about these problems or feature requests |
| `needs-reproduction`      | Likely bugs, but haven't been reliably reproduced. |
| `blocked` | Issues blocked by another issue |
| `duplicate` | Issues which are duplicates of previous issues |
| `wontfix` | Author has decided not to fix these issues |
| `invalid` | Issues which aren't valid (e.g. due to user errors). |

#### Topic Categories

| Label name | Description |
| --- | --- |
| `internal-dev` | Complex *Internal Development* discussion, not meant for new users without full code understanding |
| `documentation` | Documentation related issue/improvements |
| `performance` | Related to performance. |
| `security` | Related to security |
| `ui` | Related to visual design of the User Interface |
| `ux` | Related to the application's design in regard to the User Experience |

#### Pull Request Labels

| Label name | Description |
| --- | --- |
| `WIP` | A *work-in-progress* pull request with more changes to follow |
| `needs-review` | Pull requests which need code review, and approval from maintainers or core team |
| `under-review` | Pull requests being reviewed by maintainers |
| `requires-changes` | Pull requests which need to be updated based on review comments and then reviewed again |
| `needs-testing` | Pull requests which need manual testing |

