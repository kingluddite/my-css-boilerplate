# CSS Boilerplate

## Requirements

- node (The `npx` stands for Node Package Execute and it comes with the `npm`, when you installed npm above 5.2.0 version then automatically npx will installed)

## What this has

- box-sizing
- responsive images
- normalize.css
- live-server
- stylelint

## Install instructions

- (if you have dotfiles) Add this function to your dotfiles and call it with `$ css-boilerplate` to install all the boilerplate code
- **note** Don't forget to source the file holding this new function or it won't work (example: `$ source functions`)

```
css-boilerplate(){
  git clone https://github.com/kingluddite/eslint-boilerplate.git . && npm i
}
```

## Fix CSS code with stylelinter

`$ npx stylelint --fix "**/*.css"`

## If you are using VS Code

- Install the [ESLint package](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)
- Add these settings in the VS Code settings file📦

```
// These are all my auto-save configs
"editor.formatOnSave": true,

// turn it off for JS and JSX, we will do this via eslint
"[javascript]": {
  "editor.formatOnSave": false
},

"[javascriptreact]": {
  "editor.formatOnSave": false
},

// show eslint icon at bottom toolbar
"eslint.alwaysShowStatus": true,

// tell the ESLint plugin to run on save
"editor.codeActionsOnSave": {
  "source.fixAll": true
},

// Optional BUT IMPORTANT: If you have the prettier extension enabled for other languages like CSS and HTML, turn it off for JS since we are doing it through Eslint already
"prettier.disableLanguages": ["javascript", "javascriptreact"],
```
