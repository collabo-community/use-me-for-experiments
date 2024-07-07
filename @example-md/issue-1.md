> Note: Pull new changes in develop branch first

#### Description
In the [community app's web client](https://github.com/code-collabo/collabo-community-app), currently you have to run `npm run lint` separately in order to see warnings and/or errors being watched in the terminal. It will be nice if linting is watched and errors are displayed in the terminal too when you run `npm run dev` and the app is running. This is also similar to how angular app linting works.

#

#### Expected solution
Just like it happens in **_ts_** and **_esm_** templates in the [api-boilerplate-templates](https://github.com/code-collabo/node-mongo-api-boilerplate-templates) where linting errors is watched and shows up in the terminal when you run the dev server, In the client of our web app, we want linting to be watched and errors/warnings displayed in the terminal too when you run `npm run dev`. 

#

#### Additional context
- You may want to first test/checkout, run and make changes to the node-mongo api boilerplates, to get a better idea of how eslint works in there as described above.
- Note, the goal is not to use a tool like prettier to do the work of formatting. Do not add prettier or any tool that works like it. We just want code developers to be conscious and be mindful of the uniformity in code writing styles.
- Maybe also checkout [the package.json of the older version of the node-mongo templates](https://github.com/Ifycode-experiments/ESM-api-boilerplate-template/blob/develop/package.json), it may help.

#

#### Testing checklist
Note: Add the testing checklist below (without this note) to your pull request when submitting your fix. This will guide (you and) the contributors who will review your fix to know what is important to check or test for.
- [ ] I have tested that this eslint solution works and behaves like that of the [api-boilerplate-templates](https://github.com/code-collabo/node-mongo-api-boilerplate-templates).
- [ ] Linting is watched and errors/warnings are displayed in the terminal too when you run `npm run dev`
- [ ] I certify that I ran my checklist
