> Note: Pull new changes in develop branch first

#### Issue description
According to Nextjs documentation, [you can only use global CSS styles in the pages/_app.js file](https://nextjs.org/learn-pages-router/basics/assets-metadata-css/global-styles). 
To be able to load specific global CSS styles in the 3 different [layouts or page structure](https://nextjs.org/docs/pages/building-your-application/routing/pages-and-layouts#with-typescript) that exists in the app, we had to resort to using [styled JSX](https://nextjs.org/blog/styling-next-with-styled-jsx#writing-styles-in-external-files).
Styled JSX needs babel config to be able to work, which we have set up. But the issue is that it only works from the root of the repo. It does not work in the client folder.

#

#### Steps to reproduce this issue
- Go to https://github.com/code-collabo/collabo-community-app, and run the app locally
- Move the babel config from the root of the repo into the the client folder
- See that there are errors in the terminal and the web client app breaks

#

#### Expected behavior
Make babel config work from within the client folder, instead of from the root of the repository.

#

#### Additional context
We want to be able to achieve configuring from within project folders similar to the [api-boilerplate templates](https://github.com/code-collabo/node-mongo-api-boilerplate-templates) repo.

#

> Feel free to ask questions about this task in our discord community channel

#

#### Testing checklist
Note: Add the testing checklist below (without this note) to your pull request when submitting your fix. This will guide (you and) the contributors who will review your fix to know what is important to check or test for.
- [ ] Babel config now works from within the client folder, without breaking the client app i.e. without causing errors in the terminal.
- [ ] The styled JSX also works as it was working before. The dummy styles added before now are not broken.
- [ ] I certify that I ran my checklist
