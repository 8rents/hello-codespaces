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
2. In your browser open <https://vscode.dev>
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

## Create a new node app

In the codespaces terminal initalize a new node app `package.json` file  by running `npm init` and adjusting any of the settings.

> ### *A couple of notes about `package.json` file creation*
>
> *You can auto create a `package.json` file using `npm init -y`, however this will not create all of the options in the json array.*
>
> *You can select the default by hitting enter for each question.* ***This is better than the `-y` flag because each of the array options will be created for you.*** *You won't have to look up each of the correct key values later.*
>
> ---
>
> Here's my entry for `npm init`:
>
> - **name:** `hello-codespaces`
> - **version:** `0.0.1`
> - **description:** `An attempt at ephemeral computing by developing purely in the cloud using GitHub codespaces and vscode.dev to make a quick start node.js app`
> - **entry point:** `app.js`
> - **test command:**
> - **git repository:** `https://github.com/8rents/hello-codespaces`
> - **keywords:** `"GitHub", "codespaces", "vsCode.dev", "Ephemeral Computing"`
> - **author:** `Brenton Holiday`
> - **license:** `MIT`

## Sources

- [**vscode docs:** Developing with GitHub codespaces](https://code.visualstudio.com/docs/remote/codespaces)
- [**GitHub docs:** Introduction to dev containers](https://docs.github.com/en/codespaces/setting-up-your-project-for-codespaces/adding-a-dev-container-configuration/introduction-to-dev-containers)
- [**npm docs:** Configuring a npm package.json file](https://docs.npmjs.com/cli/v10/configuring-npm/package-json)

---

**🤍 2024 [Brenton Holiday](https://8rents.github.io)**
