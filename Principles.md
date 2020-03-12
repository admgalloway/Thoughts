# Development Principles

The following principles define my key objectives and approaches when building software. I try to keep these at the forefront of any work I do and promote them wherever I go.

In practice there are many standards, patterns and processes that I use and follow when building software, these simply capture the characteristics of the solutions I want to produce.

## Keep it simple.

#### Clean code beats clever code.

When your focused on a problem it’s easy to know the solution inside-out for a few days whilst your working on it. Will you still remember it as well in 6 months’ time? Maybe. Your colleagues definitely wont.

Write self-documenting code wherever possible - descriptive variable names and readable logic checks can replace lengthy comments or verbose explanations. Avoid obscure one-liners where possible – they’re difficult to read and make it tricky to debug issues.

Extension methods, generics and abstract classes can be great for simplifying and sharing code, but care must be taken to ensure they are well documented and easy to follow. At the very least, each method should include a descriptive summary, and if it isn't explicitly obvious to another developer how a solution works then include a link to a document that will provide the additional information they'll need.

Writing maintainable code should be a top priority, so take time to refine your solution into readable code that you – or anyone else – will be able to return to and understand in the future.

## Consistency is key.

#### And collaboration is key to consistency.

Consistency is critical when it comes to maintaining software systems. A modern development team will change and grow quickly and it's important everyone contributes work that others can support.

This doesn't just account for coding styles - server names, repos, documentation, project architecture, build/deployment tasks - the more you stick to consistent patterns the quicker and easier you and your colleagues will be able to adapt to new projects. Picking up a ticket to update an API you've never worked on before? Doesn't matter, before even cloning that repo you should know what the general project structure is, where to find settings, business logic or data access code, leaving you free to jump straight in to understanding what the code itself is doing.

As a team, agree on a set of standards you want to meet and document them. Make it a team mandate and everyone will feel their adhering to their own standards rather than having someone else's preferences enforced on them. The key thing here is not the conventions themselves, its consistent use of them. 

Consistency is also crucial for the next design principle - automate everything. Keeping to consistent naming conventions and patterns allows us to re-use convention-based automation scripts without lengthy or verbose configuration.

## Automate everything.

Development is often a series of repetitive or time-consuming tasks, but the tools we have available today are incredibly powerful and you should take advantage of them where possible.

There aren't many processes that don't have room for automation. Deployments, provisioning and testing are all fairly standard practice now, but if you find yourself spending time on the same tasks then there's a good chance others are too - can you write a PowerShell or Bash script to do that for you? What about IDE templates that generate skeleton architectures for new projects, saving on the old copy-paste-rename job and cutting down on those "sprint zero" tasks! 

Can your coding skills and technical knowledge help others in the business? If you see someone spending hours of their day or week collating information or reports for example, then see what you can do to help out. An hour of your time could save many more of theirs, and they're then free to make you coffee when you need it, result!

You're also not going to be here forever, and it's important you leave solutions in a better state than you found them. Automating routine and business-critical tasks can continue running once your gone, and self-documented scripts can be a great way of cetralising and retaining knowledge or capabilities within the team. 

I, for one, welcome our new robot overlords.

## Rome wasn’t built in a day.

#### But they were laying bricks every hour.

As developers we tend to strive for that Utopia solution, where every line of code is a beautify-crafted and carefully-considered masterpiece. Or at least, where the same naming conventions are followed from one class to the next... In reality there will always be compromises required to deliver solutions - deadlines, late requirement changes, inconsistencies in implementations.

You can't control it all, but you can plan for those eventualities - identify technical priorities and be assertive in delivering them. Decide what you can afford to compromise on and plan to change it later. Just by doing that you will consider what you want to achieve and the impact it will have on your code, and make it easier to accommodate changes in the future.

Don't expect to deliver your perfect solution on day one. It takes time, effort and refinement to get right, but where possible aim to deliver one area of work from every single project that contributes to the greater good of the team or platform - a reusable code library/package, a build template, an automated process step. Whatever it is, if you adding to the ecosystem as you go then you'll get to where you want to be quicker.
