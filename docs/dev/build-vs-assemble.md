# Build vs Assemble

The Foam prototype is built by assembling third-party extensions, which seems like a good strategy because

- It supports picking and mixing of tools and workflows
- Less code to write and maintain

But there's also a bunch of roadmap items that are hard to implement this way, as the third party plugins don't do exactly what we want them to do (e.g. Markdown All In One is not compatible with [[referencing-notes-by-title]].

Overall, we should strive to build big things from small things. Focused, interoperable modules are better, because they allow users to pick and mix which features work for them. A good example of why this matters is the Markdown All In One extension we rely on: While it provides many of the things we need, a few of its features are incompatible with how I would like to work, and therefore it becomes a limiter of how well I can improve my own workflow.

However, there becomes a point where we may benefit from implementing a centralised solution, e.g. a syntax, an extension or perhaps a VSCode language server. As much as possible, we should allow users to operate in a decentralised manner.
