# Building p5.js Web Editor from Source
## Build Process
Following the [p5.js Contributor guidelines](https://p5js.org/contribute/contributor_guidelines/#quick-get-started-for-developers) and [Development Installation instructions](https://github.com/processing/p5.js-web-editor/blob/develop/contributor_docs/installation.md), I was able to build the p5.js Web Editor from source — albeit with some limited functionalities. The first steps of installing Node.js, forking the p5.js Web Editor repository, and cloning [my fork](https://github.com/callybton/p5.js-web-editor) into my local computer were straightforward. Some issues began to arise in installing all the dependencies with `npm install`.
```
npm WARN EBADENGINE Unsupported engine {
npm WARN EBADENGINE   package: 'execa@8.0.1',
npm WARN EBADENGINE   required: { node: '>=16.17' },
npm WARN EBADENGINE   current: { node: 'v16.14.2', npm: '8.5.0' }
npm WARN EBADENGINE }
npm WARN EBADENGINE Unsupported engine {
npm WARN EBADENGINE   package: 'human-signals@5.0.0',
npm WARN EBADENGINE   required: { node: '>=16.17.0' },
npm WARN EBADENGINE   current: { node: 'v16.14.2', npm: '8.5.0' }
npm WARN EBADENGINE }

up to date, audited 3522 packages in 6s

416 packages are looking for funding
  run `npm fund` for details

112 vulnerabilities (5 low, 45 moderate, 60 high, 2 critical)
```
The *Development Installation* instructions only required Node.js version 16.14.2, so I simply proceeded. (As I'm focusing on the fundamental build, I decided to revisit addressing vulnerabilities in the future.) Afterward, I used `npm start` to successfully run the p5.js Web Editor on a local server.
![Screenshot of p5.js Web Editor running on local server.](https://github.com/bennColl-cs4387/camisola/blob/c9c82eeb4f3212bfd1e7cbe6e4f9b680abd16ccb/Week%205/p5js%20Web%20Editor%20-%20Local%20Host.png)


## Changed Code
After building the p5.js Web Editor from source, I tested out implementing basic modifications to the code. I looked through my cloned repository and found the stylesheets. In *client/styles/components/_editor.scss*, I changed the text editor's background color to verify if my changes would appear once I refreshed my browser: this proved successful.
![Screenshot of p5.js Web Editor running on local server, with changed code.](https://github.com/bennColl-cs4387/camisola/blob/d6daae76572f2f8e32f110a208c9c42d411cc66f/Week%205/p5js%20Web%20Editor%20-%20Changed%20Code.png)
