# Tailwind CSS @apply Directive Conflict

This repository demonstrates a common issue when using Tailwind CSS's `@apply` directive: conflicting styles.

When multiple classes with conflicting styles are applied using `@apply`, the last one applied takes precedence.  This can lead to unexpected visual results if not carefully managed.

The `bug.css` file showcases the problem, while `bugSolution.css` demonstrates a possible solution.

## Bug
In `bug.css`, applying `text-red-500` and `text-blue-500` using `@apply` results in blue text, as `text-blue-500` is applied last.

## Solution
`bugSolution.css` demonstrates solutions: using more specific selectors to avoid the conflict, or carefully managing the order of `@apply` directives.