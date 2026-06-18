## Git Commit Message Guidelines

Zenolith uses human-readable Git commit messages. Commit messages should explain the intent behind a change and keep the project history easy to review.

### Format

Separate the commit subject from the body with a blank line:

```txt
Summarize changes in around 50 characters or less

Explain what changed and why. Wrap body text at around 72
characters when possible.
```

### Subject line

The commit subject should:

* Be around 50 characters or less when practical
* Start with a capitalized word
* Not end with punctuation
* Use the imperative mood

Good examples:

```txt
Add SVG marker support
Fix theme override precedence
Document GitHub Pages deployment
Refactor flowchart parser diagnostics
```

Avoid:

```txt
Added SVG marker support.
Fixes theme stuff!
Updated files
```

### Body

Use the body when the change needs context.

The body should explain:

* What changed
* Why the change was made
* Any important side effects or tradeoffs

The body should avoid explaining implementation details that are already clear from the code.

### Example

```txt
Fix theme override precedence

Custom theme classes should override built-in theme classes so users
can safely extend Zenolith without fighting the default styles.

This keeps class-based theming predictable and preserves the documented
override behavior expected by downstream renderers.
```

### Reviewer line

When requested, include a reviewer line at the end of the commit body:

```txt
CR: @reviewer-one, @reviewer-two
```

The `CR:` line should be separated from the rest of the body by a blank line.
