# Writing a good commit message

### Rules

- Max 50 characters

```
Bad
git commit -m "This is a long commit message. It should not be this long, the description should be in the commit's body."

Good
git commit -m "Remove deprecated methods"
```

- No punctuation

```
Bad
git commit -m "Refactor system X."

Good
git commit -m "Refactor system X"
```
- Imperative writing

```
Bad
git commit -m "Fixed bug X"

Good
git commit -m "Fix bug X"
```

### Test a commit subject this way:

*"If applied, this commit will [subject]."*

The commit subject should fit this sentence.

### Atomic commits

[Source](http://www.freshconsulting.com/atomic-commits/)

> The common thought with those new to source control is to commit “at the end of the work day”, or “whenever I feel like it”, or whenever a batch of fixes are complete. Avoid those pitfalls and consider what an “atomic” block of work is and make a commit only when that is complete.

> When working with new features, an atomic commit will often consist of multiple files, since a layout file, code behind file, and additional resources may have been added/modified.

- Commit each fix or task as a separate change
- Only commit when a block of work is complete
