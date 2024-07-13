> Note: Pull new changes in develop branch first

#### Description
We want to be able to run a github action workflows against the [collabo community app](https://github.com/code-collabo/collabo-community-app) repo's client, that checks the compatibility of contributor's submissions with different nodejs versions. 

We want this workflow to run when:
- When contributors **_send PR_** to the **main** or **develop** branch of the collabo community app repo
- When contributors **_push_** to the **main** or **develop** branch in the collabo community app repo

Nodejs versions to run the github actions workflow for:
-  node-version: [16.x, 17.x, 18.x, 19.x, 20.x]

#

#### Take a clue from these files from other repos
- **node-mongo-cli:** https://github.com/code-collabo/node-mongo-cli/blob/develop/.github/workflows/node.js.yml
- **node-mongo-api-boilerplate-templates:** https://github.com/code-collabo/node-mongo-api-boilerplate-templates/blob/develop/.github/workflows/node.js.yml

#

#### Additional context
You may want to send a dummy PR to either the **node-mongo-cli** or the **node-mongo-api-boilerplate-templates** to just see and test how github actions work. Once you send the PR there, towards the bottom of the PR you will notice the checks against different nodejs versions.

#

#### Testing checklist
Note: Add the testing checklist below (without this note) to your pull request when submitting your fix. This will guide (you and) the contributors who will review your fix to know what is important to check or test for.
- [ ] Necessary config file have been added in the correct folder and/or position in the community app repo
- [ ] Configuration covers **_sending PR_** to the **main** or **develop** branch
- [ ] Configuration covers **_pushing_** to the **main** or **develop** branch
- [ ] Configuration covers node-version: [16.x, 17.x, 18.x, 19.x, 20.x]
- [ ] Workflow runs (at the bottom of the PR submitted)
- [ ] I certify that I ran my checklist
