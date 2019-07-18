#  BlueGenes MSA Viewer

BlueGenes MSA Viewer is a tool made for BlueGenes following BlueGenes Tool API. It can help users (biologists) to view [Multiple Sequence Alignment](https://en.wikipedia.org/wiki/Multiple_sequence_alignment) of Proteins. It can also be used as standalone tool to integrate in any web application.

### Before deploying to BlueGenes (or anywhere)

1. Make sure to deploy an instance of [sequence-alignment](https://github.com/intermine/sequence-alignment-service) service
2. Then update the base url in this tool to the deployed url in `src/sequence-align-service.js`
3. Build the tool using `npm run build`
4. Deploy where ever you want! :D

### To set up locally for development

1. Clone the repo
2. `cd bluegenes-msa-viewer` and then `npm install` to install dependencies.

All of the editable source files for css and js are in `src`. To bundle for prod, run the following commands:

#### CSS

Assuming [less](http://lesscss.org/) is installed globally:

```
npm run less
```

#### JS

Assuming [webpack](https://webpack.js.org/) is installed globally:

##### Single build:
```
npm run build
```


##### Applied Coding practices / ESLint Rules:
- _indent_: use __tab (2 space tab)__ instead of spaces to not get an error.
- _linebreak-style_: use __\n__ for a newline, if you're on windows, configure it in your editor settings.
- _quotes_: use __single quote__ instead of double quote.
- _semi_: use _semi colon_ at end of each statement / expression / function definition.
- _comma-dangle_: do not use dangling commas i.e. extra comma at the end of object values, function args, etc.). More about this [here](https://eslint.org/docs/rules/comma-dangle).
- More pre-configured rules from __eslint:recommended__ you must follow to not get errors [here](https://eslint.org/docs/rules/).

##### Developing:
Run each of these commands in separate terminals:

To rebuild your js every time you save:

```bash
npm run dev
```

To serve your page at [http://localhost:3456](http://localhost:3456):
```bash
npm run server
```
