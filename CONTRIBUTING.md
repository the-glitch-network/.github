# How to contribute to The Glitch

Thank you for taking the time to contribute! There's a few small steps you may want to go over before starting to
contribute.

1. Check to see if there's already an existing pull request on the repository for what you want to do, or issue for a
   bug or request you want to submit.
    - This helps prevent you from needlessly doing work that's already been done. If you think the current PR is unfit,
      or could use some fixing, give constructive criticism and suggest fixes by sending in a code review or a comment.
    - If the issue doesn't seem to fit in all what you wanted to submit, or is missing details, you can go ahead and add
      on to the issue.
2. If it's a new feature, see if it'll be within scope of the project.
    - If you're unsure, you can always open a discussion on the repository, if it's enabled of course, check for all
      issues with the label of `enhancement`
      and `feature request`, or ask within the [development server](https://discord.gg/EmPS9y9).
3. If there's no preexisting pull request or issue, and there's no hitch you holding back, submit a new PR or issue.

If you'd like to talk about development for The Glitch, or need an issue resolved,
join [KJP12's development guild](https://discord.gg/EmPS9y9).

[![KJP12 Development](https://discord.com/api/guilds/380201541078089738/widget.png?style=banner2)](https://discord.gg/EmPS9y9)

## Reporting a bug

1. **Check existing issues first.** Make sure the bug wasn't already reported before.
    - If the bug was already reported before, and the issue is still open, add any additional details that may otherwise
      be missing in its issue.
2. **Have reproducible steps for the bug.** Nothing's worse than tracking down a Heisenbug, a sort of Schrödinger's bug.
    - If you cannot get any reliably reproducible steps, try to at minimum give anything that maybe useful such as a
      crash report, and what operating system you're using.
3. **Provide as much detail as possible.** Use the forms we've provided to help yourself out in knowing what data to
   provide.

## Code & Embedded Documentation

1. **Check existing PRs first.** Make sure that there isn't already one for what you want to change or add.
    - If the PR already exists, suggest changes on that PR instead, and save yourself the work.
2. **Fork the repository** you want to contribute your changes to. If you'd like us to help you make changes, fork to a
   user account rather than an organisation. Sometimes this maybe easier than a back & forth.
3. **Make your changes.** Please follow the codestyle of the surrounding structure & classes.
    - If the repository has Spotless, Prettier or similar, you will have to run that after you're done to make the code
      pass the checkstyle. Some older, more complex repositories will not have a checkstyle and may require you to
      manually make the code match the surrounding.
4. **Document your new code,** including functions, classes and fields. Java projects use standard Javadocs for
   documentation.
    1. Ensure that the Javadoc describe what it does in whole, and for complicated or implementation-dependent methods,
       describes how the method functions, and what it does in detail. This maybe important for larger PRs to be
       accepted.
    2. Be sure to attribute yourself within the Javadoc. If it's a new class, setting the `@author` tag only on the
       class is sufficient, unless otherwise required by the codestyle or integrated libraries such as Mixin. If you're
       adding a function to a preexisting class that wasn't created by you previously, and the method is over 4 lines,
       both the
       `@author` and `@since` tags are required.
    3. Include `@param`, `@return`, `@implSpec`, and `@implNote` as needed. These are helpful for people who need to use
       the method in the future, but don't necessarily want to read the source code to understand it. If it is useful to
       know about the classes to use the class or method, include `@see` tags, and inline links as
       `{@link Class#method()}` around the documentation as required.
5. **Commit your changes.** [Be sure your commit summaries are useful.](https://cbea.ms/git-commit/)
   Committing semi-regularly for larger PRs may prove useful for keeping the summary sane. You may write in greater
   detail what the commit contains, but that isn't necessary for messages that the summary describes the whole commit.
    - A summary is the first line of the commit message. It must be shorter than 75 characters, and should be in
      imperative mood, i.e. `Add a potato` rather than `Adds a potato` or `Added a potato`.
6. Submit a PR to the repository you forked.
    - If needed, you're free to force-push & rebase your code as needed to simplify commit history, code, and whatnot.