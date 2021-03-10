# TAU Test Automation for Accessibility

- [Web UI Python Path](https://testautomationu.applitools.com/learningpaths.html?id=web-ui-python-path)
- [Test Automation for Accessibility with Marie Drake](https://testautomationu.applitools.com/accessibility-testing-tutorial/)  
- [WCAG 2.1](https://www.w3.org/TR/WCAG21/)
- [Conformance Levels](https://www.w3.org/WAI/WCAG21/Understanding/conformance/)

## Resources for this course

- Node and NPM must be installed - [Node and NPM can be downloaded here](https://nodejs.org/en/download/)
- [Axe-CLI](https://github.com/dequelabs/axe-cli)

## Trouble Shooting

While installing `Axe-CLI` I encountered an error `cb.apply is not a function`, I used the below website to help resolve this issue which seem to stop the error, specifically option one - https://github.com/nodejs/help/issues/2874#issuecomment-663661148

- [Help resolving errors when running npm install -g axe-cli](https://github.com/nodejs/help/issues/2874)

## Commands

- To install `Axe-CLI` run the command `npm install -g axe-cli`
- Checking node version run `node -v`
- This command will run chrome in headless mode by default `axe mariedrake.com` this will produce a report in the terminal, providing links to direct you to how to resolve the issue
- `axe http://mariedrake.com --browser chrome` - Launches Chrome
- Multiple pages can be passed in, comma separated - `axe http://mariedrake.com, mariedrake.com/about --browser chrome`
- Disabling rules, whilst it isn't advised, it is possible `axe mariedrake.com, mariedrake.com/about --browser chrome --disable link-name`
- Saving output `axe mariedrake.com, mariedrake.com/about --browser chrome --save test-results.json` give output in your file
