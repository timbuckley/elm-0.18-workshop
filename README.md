<i>This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a> - except for the `server/` directory, which has its own license. Many thanks to those who [wrote the server](https://github.com/gothinkster/moleculer-node-realworld-example-app)!</i>

Getting Started
===============

## Install Elm Tools

1. Install [Node.js](http://nodejs.org) 7.0.0 or higher

2. Add a plugin for your editor of choice: [Atom](https://atom.io/packages/language-elm), [Sublime Text](https://packagecontrol.io/packages/Elm%20Language%20Support), [VS Code](https://github.com/sbrink/vscode-elm), [Light Table](https://github.com/rundis/elm-light), [Vim](https://github.com/lambdatoast/elm.vim), [Emacs](https://github.com/jcollard/elm-mode), [Brackets](https://github.com/lepinay/elm-brackets)

3. Not required, but **highly** recommended: enable "[`elm-format`](https://github.com/avh4/elm-format) on save" in your editor.

4. Run the following command to install all the other Elm tools:

> **Note:** Make sure not to run this command with `sudo`! If it gives you an `EACCESS` error, apply [**this fix**](https://docs.npmjs.com/getting-started/fixing-npm-permissions#option-two-change-npms-default-directory) and then re-run the command (still without `sudo`).

```shell
npm install -g elm elm-test elm-live@2.7.5 elm-format@exp
```

You can confirm this worked by running:

```shell
elm --version
```

It should print `0.18.0` if everything worked!

## Clone this repository

Run this at the terminal:

```shell
git clone https://github.com/rtfeldman/elm-0.18-workshop.git
cd elm-workshop
```

> **Note:** Tab characters are syntax errors in Elm code, so if your editor uses them for indentation, definitely switch it to spaces for this workshop!

## Start the server

We'll be running a local server for our Elm UI to use. Let's get it set up.

```shell
cd server
npm install
npm run dev
```

If the server started up successfully, you should see `mol $` at the end of your terminal.

We're going to leave this server running and not touch it again for the duration
of the workshop, so **don't close it** until the workshop is over!

## Build the Elm UI

Leave the existing terminal running, and open a **second** terminal.

In the new termnal, `cd` into the `elm-workshop` directory again.

Then run this to build the Elm code for the first time:

```shell
elm live Main.elm --output=public/elm.js --open
```

A browser should open, and you should see this in it:

<img width="375" alt="A screenshot showing “You’re all set!”" src="https://user-images.githubusercontent.com/1094080/39399636-63605a72-4aef-11e8-82bc-2b94e85369d1.png">

If things aren’t working, the instructor will be happy to help!

## Links

* [Slides](https://docs.google.com/presentation/d/1sNx5k3_fHwJcgm9QEY1LsMH_TyF5SnnOSDKb8HvFsEU/edit?usp=sharing) accompanying this workshop, including speaker notes in case you’d like to [run this workshop yourself](https://github.com/rtfeldman/elm-0.18-workshop/blob/master/TEACHING.md)
* [Elm in Action](https://www.manning.com/books/elm-in-action?a_aid=elm_in_action&a_bid=b15edc5c), a book by [Richard Feldman](https://twitter.com/rtfeldman), creator of this workshop
* [Official Elm Guide](https://guide.elm-lang.org/) by [Evan Czaplicki](https://twitter.com/czaplic), creator of Elm
* [Elm Slack](http://elmlang.herokuapp.com/) - amazingly helpful chat community. People in [the `#beginners` channel](https://elmlang.slack.com/messages/C192T0Q1E/) are happy to answer questions!
* [Elm Discourse](https://discourse.elm-lang.org/) - for longer-form discussions.