# hello-codespaces

> *An attempt at ephemeral computing by developing purely in the cloud using GitHub codespaces and vscode.dev to make a quick start node.js app*

---

## Using vscode.dev as an IDE

We will use GitHub as a file system and vscode.dev as an IDE

1. Create a new repository on GitHub
    - Add a Name (mine's called `hello-codespaces`)
    - Add a description
    - Add a README
    - Add a license
    - Add a Node GitIgnore to the Repo
2. In your browser open: **<https://vscode.dev>**
    - Sign in with GitHub and/or Microsoft
    - Open the GitHub Repo you just made
    - Type any additional documentation into the README.md file
    - Commit and push the "initial commit"
    - When you refresh your github repo in your browser we will see the changes

## Using Codespaces as a development enviornment

1. Open a new terminal window in vscode
2. Click the "continue working in GitHub Codespaces" button
3. Authorize Codespaces
4. Select the type of server you want to spin up
5. A new window will open with a terminal
6. Test that node is installed `node -v` prints out `v20.17.0`

## Create a new node app `package.json` file

The `package.json` file is the heart of any nodejs project. It contains all meta data about the project, any dependencies, version number, keywords, etc...

In the codespaces terminal you can initalize a new `package.json` file by running `npm init` and adjusting any of the settings.

> ### *A couple of notes about `package.json` file creation:*
>
> *You can select the default answer for each question by hitting `enter` as they come up.*
>
> *You can completely auto create a `package.json` file with  `npm init` using the `-y` flag, however this will not create all of the options in the json array. ***Any values that are not created when the `package.json` is made will have to have the correct keys looked up later when needed.***

When creating my package file I just hit enter all the way through except for the `entry point` question which I changed from `index.js` to `app.js`.

I also entered my GitHub repo and changed the version number to `0.0.1`.

## Creating a `.devcontainer` file

The `.devcontainer` file contains all of the information needed for the environment of your application. 

Select the `<> Code` dropdown on your GitHub repository page, then `codespaces` then on top where it says "codespaces: your work in the cloud", click the `...` button and select "configure dev container".  

This will create a file in your repo `*your-repo-name*/.devcontainer/.devcontainer.json`.

In search box on the right select what kind of system you will need. I simply searched "node" and selected **"Node.js (via nvm), yarn and pnpm"** from there it provides instructions on editing your `.devcontainer.json` file.

> Copy and paste the following snippet into the features attribute of your devcontainer.json file.

```bash
"ghcr.io/devcontainers/features/node:1": {}
```

So your file would look something like:

```
// Features to add to the dev container.
// More info: https://containers.dev/features.
"features": "ghcr.io/devcontainers/features/node:1",
```

## Sources

- [**vscode docs:** Developing with GitHub codespaces](https://code.visualstudio.com/docs/remote/codespaces)
- [**GitHub docs:** Introduction to dev containers](https://docs.github.com/en/codespaces/setting-up-your-project-for-codespaces/adding-a-dev-container-configuration/introduction-to-dev-containers)
- [**npm docs:** Configuring a npm package.json file](https://docs.npmjs.com/cli/v10/configuring-npm/package-json)

---

**🤍 2024 [Brenton Holiday](https://8rents.github.io)**
