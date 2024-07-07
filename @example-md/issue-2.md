> Note: Pull new changes in develop branch first

#### Bug description
We have a `PageHeadElement` component that helps us change the title tag content for our web app in the user's browser tab. 
With what we have in the code currently, when you switch routes/pages through typing or pasting url in the browser, the transitioning of the title content in the browser tab is not smooth. There's some flicker.

#

#### Steps to reproduce the buggy behaviour

1. Run the web app: https://github.com/code-collabo/collabo-community-app
2. change to the available routes in the browser:
    - /community
    - /code-collabo/overview
    - /code-collabo/projects
    - /other-subcommunity/overview
3. Observe the page title as it changes in the browser tab, see that the title change/transition is not smooth and there is some form of flickering.

#

#### Expected behavior
Smooth change in page title in the browser tab when changing routes

#

> Feel free to ask questions about this task in our discord community channel

#

#### Testing checklist
Note: Add the testing checklist below (without this note) to your pull request when submitting your fix. This will guide (you and) the contributors who will review your fix to know what is important to check or test for.
- [ ] Smooth change in page title in the browser tab when changing routes
- [ ] The `PageHeadElement` component is retained as the component where the title tag resides even as the title changes
- [ ] I certify that I ran my checklist
