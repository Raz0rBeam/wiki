# 📖 BSMG Wiki &nbsp;[![CI Status](https://github.com/bsmg/wiki/workflows/Wiki%20CI/badge.svg)](https://github.com/bsmg/wiki/actions)
## ✏️ Contributing
If you wish to contribute, [submit a pull request](https://github.com/bsmg/wiki/pulls) with your changes. A wiki maintainer will review your contributions and merge them in if deemed appropriate.  

Don't know where to start? Checkout this [crash course](https://docs.google.com/document/d/1r6IP6l3uo8rc__GxfLkpaToxheeXotdYaKEj3oWB2js/edit?usp=sharing) on making contributions!

Alternatively, users who are unsure on how to work with Git can [submit an issue](https://github.com/bsmg/wiki/issues) that contains a link to a shared google document with the text you would like to contribute. Note this will take longer to process than submitting a pull request.  

### 🌐 Localization &nbsp;[![Crowdin](https://badges.crowdin.net/bsmg-wiki/localized.svg)](https://crowdin.com/project/bsmg-wiki)
Translation efforts are managed using [Crowdin](https://crowdin.com/project/bsmg-wiki).
There you can see the status of each language available that needs translating. 

#### Want to Help Translate?  
[Apply Here](https://forms.gle/e3BqA3poMjESARe76) and make sure you are in the [BSMG Discord](https://discord.gg/beatsabermods). We will be in touch!

If you don't see your language available on Crowdin you can still [apply](https://forms.gle/e3BqA3poMjESARe76) and we will add it once you are accepted!

## 🧪 Development
To run a local copy of the wiki:
1. Install [Node.js](https://nodejs.org/en/download/)
2. Install [Yarn](https://yarnpkg.com/getting-started/install)
3. [Fork this repo](https://guides.github.com/activities/forking/), then clone it. **Make sure to do all work on [another branch](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/creating-and-deleting-branches-within-your-repository#creating-a-branch).**
4. Open a command-line window in the directory you just cloned into, then run the command `yarn` to install required packages.
5. After packages are installed, start the development server with the command `yarn dev`. You can kill the server by closing the terminal or by pressing <kbd>CTRL+C</kbd>
    * If you run into an error when trying to use `yarn dev` on Windows, try taking out `yarn.ps1` and `yarnpkg.ps1` in `user/Appdata/Roaming/npm`. 
6. Open the link to [`localhost`](http://localhost:8080/) that appears in the console once the development server is running.

When you make changes to your local wiki files, the local website will update those pages as soon as they are saved! **Note:** Sidebar headers do not change due to an issue with Vuepress. They will render correctly if you restart the dev server, and on the final build.

The Wiki has a built-in linter that runs automatically when you push commits to enforce formatting rules. You can run this on your local copy with the command `yarn lint` to flag issues. You can also run `yarn run lint:markdown --fix` to have the linter try to resolve the issues automatically. If you need assistance with interpreting or fixing the errors, [submit an issue](https://github.com/bsmg/wiki/issues) with a screenshot of the errors attached.

Once you have finished making changes, you can either commit them directly using `git` tools, or copy them into the GitHub web interface if you don't know how to use `git`.

## 🚀 Deploying
The wiki is deployed using Docker. Pull the [latest image](https://github.com/bsmg/wiki/packages/54581) and run it. It exposes port 80, which can be remapped to whatever.

## 🔐 Licensing
* The code that generates the wiki is licensed under the [MIT License](https://github.com/bsmg/wiki/blob/master/LICENSE).  
* The wiki content is licensed under the [Creative Commons BY-NC-SA 4.0 License](https://github.com/bsmg/wiki/blob/master/wiki/LICENSE).  
* Translations of the wiki content is owned by the Beat Saber Modding Group (BSMG) and licensed under the [Creative Commons BY-NC-SA 4.0 License](https://github.com/bsmg/wiki/blob/master/wiki/LICENSE).
