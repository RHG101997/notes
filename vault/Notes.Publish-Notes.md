---
id: AXP8DZ5DgD9L4h4a2gO0u
title: Publish-Notes
desc: ''
updated: 1639766960238
created: 1639766242076
---


## How to publish my Notes(Remainder):

Here I will save several of the commands that are required to publish my notes to public. Also to get the most up to date notes please `git clone` the repository since the procedure for publishing needs to be performed by a computer that has all the requirements. Explain in the next section.

References: [Here](https://wiki.dendron.so/notes/23a1b942-99af-45c8-8116-4f4bb7dccd21/)

### Requirements:

* `Node.js` is required
* Intallation of `dendron-cli`

```bash
# intall
npm install -g @dendronhq/dendron-cli
# upgrade
npm install -g @dendronhq/dendron-cli@latest

```

* Setup if it is the first time running in this workspace. Initialize dendron-cli

```bash
# Init nodejs
npm init -y 
# install in directory
npm install @dendronhq/dendron-cli

# Update .gitignore
echo .next >> .gitignore
# Clone the nextjs repository and install dependencies
npx dendron publish init
```




### Publishing Commands

For building and Previewing( `https://localhost:3000`):

```bash
npx dendron publish dev
```

For publishing we need to run a export with a `github` target:

```bash
dendron publish export --target github

# Deployment
git add .
git commit -m "dendron page update"
git push
```

After this the website should update in a few seconds.