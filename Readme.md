# Search Engine Response Page

## Demo
[https://agitated-kirch-8767cd.netlify.app](https://agitated-kirch-8767cd.netlify.app)

SERP is a Trie + levenshtein distance based, mobile-ready, localstorage run, bootstrap - Jquery powered Search engine response page which comes with default dataset of some marvel characters and lets you add/index your own entries and stores them on browser's localstorage for you to use later. Keep in mind, it doesn't have a backend and hence any entry made will only be available on same device (just trying to display search capabilties using pure javascript)

## Features

- Lists all searchable entries
- Let's you add into searchable entries by submiting simple form that stores your entry into localstorage
- Remembers your search history
- gives search suggestions as you type
- autocorrects (Did you mean "XYZ") when you searched with wrong spellings


## Tech

SERP uses a number of open source projects:

- [Twitter Bootstrap](https://getbootstrap.com) - great UI boilerplate for modern web apps and to make the UI responsive!
- [JQuery](https://jquery.com) - Primarily for the ease of DOM manipulation
- [autosuggest-trie](https://github.com/moroshko/autosuggest-trie) - Minimalistic trie implementation for autosuggest and autocomplete components in pure javascript.
- [Browserify](http://browserify.org) - Browserify lets you require('modules') in the browser by bundling up all of your dependencies. It is used to bundle autosuggest-trie and js-levenshtein to be used on browsers.
- [js-levenshtein](https://github.com/gustf/js-levenshtein) - Pure JS implementation calculating the Levenshtein distance between two strings.

## Installation

SERP requires [Node.js](https://nodejs.org/) and [npm](https://www.npmjs.com/) to install and bundle JS dependecies.

Install the node and npm if it is not installed and do the following.

```
npm install -g browserify
npm install autosuggest-trie
npm install js-levenshtein
```

Once installed, move ahead to bundle the dependencies with browserify:

```
browserify main.js -o bundle.js
```

## Deployment

You are free to deploy and host it with absolutely any hosting/web service. The repository has index.html which serves as default page and is implicitly recognised as default home page of any hosted web whereever you deploy it. 

For simplicity, you can just clone the repo make your own changes as you need and use your own repo with netlify or similar services to link your github repository for an automated github event trigger based continuous deployment.

to know more follow step by step guide here: https://www.netlify.com/blog/2016/10/27/a-step-by-step-guide-deploying-a-static-site-or-single-page-app



## License

MIT

**Free Example Implementation, Hell Yeah!**