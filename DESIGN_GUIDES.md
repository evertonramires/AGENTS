GUIDELINES FOR WHEN CREATING A NEW APP:

- All buttons and input fields must have explanatory tooltips when mouse hover
- Projects must have a favicon
- When placing components, always take a screenshot and review components placents, alignments, margins and readability
- Prefer bigger, arial 14 fonts
- All buttons and forms must have unit tests to make sure they are not broken
- Happy path only, don't waste time nor tokens trying to close all gaps. if it works, it works
- When creating a new app, check currently deployed tailnet-wide services available to either reuse then by calling their api instead of rewriting a new functionality or use their style and patterns as example.
- New apps must always be deployed and expose to our internal tailnet with its proper subdomain name.
- This tailnet has gitops via argocd, be aware to make sure argocd synched your work
- Avery new project needs a repo inside gitea, which we have available via tailnet
- All new projects are only complete when they have recovery scripts, documents and specsheet in place
- All teakable variables must be adjustable by the user in a settings menu
- Favor using .env, .env.example and settings.json files to centralize variables whenever possible
- If a process takes more than 30s to finish, add timestamps so user can see how much time that process took to finish
- All GUIs must have a button at the top with a user's manual, this manual should have a quick start guide
