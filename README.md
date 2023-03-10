# DocsifyJS Template 📒 🕸
> Starter template for a Markdown-based docs site

[![GitHub tag](https://img.shields.io/github/tag/abpanic/docsify-js-template)](https://github.com/abpanic/docsify-template/tags/?include_prereleases&sort=semver)
[![License: Unlicense](https://img.shields.io/badge/license-Unlicense-blue.svg)](http://unlicense.org/)

[![Made with latest Docsify](https://img.shields.io/badge/docsify-v4-blue?label=docsify)](https://docsify.js.org/ "Go to Docsify website")
[![Hosted with GH Pages](https://img.shields.io/badge/Hosted_with-GitHub_Pages-blue?logo=github&logoColor=white)](https://pages.github.com/ "Go to GitHub Pages docs")


## Preview

<div align="center">
    <a href="https://abpanic.github.io/docsify-js-template/">
        <img src="/sample.png" alt="Sample screenshot" alt="Go to website" width="500" />
    </a>
</div>

<br>

<div align="center">

[![View site - GH Pages](https://img.shields.io/badge/View_site-GH_Pages-blue?style=for-the-badge)](https://abpanic.github.io/docsify-js-template/ "Go to website")

Instead of forking, rather make a new repo using this template button:

[![Use this template](https://img.shields.io/badge/Generate-Use_this_template-2ea44f?style=for-the-badge)](https://github.com/abpanic/docsify-template/generate)

</div>

If you want to improve the original template, then fork it and make a PR.


## Features

- 🏭 Template for a SPA modern docs site.
- 📗 Use your awesome project's _existing_ markdown files.
- 🤩 Light on code – just add a single HTML file and optionally add cover page and navbar config.
- 🚀 Easy to host as a static site on GitHub Pages. No build step needed.


## Purpose
> How to use this project

- Create a **new repo** from the template and host it on GitHub Pages immediately. This is good for trying out Docsify or building a site project from scratch.
- Use this project as a **base** - follow instructions to download just the necessary files to your _existing_ repo's `docs` directory
- View the **live** demo site to see what you'll get.

For more info on Docsify, see my [DocsifyJS Tutorial](https://learn-docsify.netlify.app). That covers intro to DocsifyJS, including installation, running and configuration. If you look at the repo, that has has more content and configuration than this relatively plain template site.

[DocsifyJS Tutorial]: https://learn-docsify.netlify.app/#/


## How to use Docsify in your projects

### Copy files

Use one of the approaches below to setup Docsify in your own project.

#### A. Use this template

Create a _new_ forked project based on this template  by clicking the button below. You'll get a fork in your own repo.

[![Use this template](https://img.shields.io/badge/Use_this_template-2ea44f)](https://github.com/abpanic/docsify-template/generate)

You could start adding code outside of the _docs_ directory, however this project is intended as a standalone docs site which can be configured for experimentation and used as reference.

#### B. Add Docsify to an existing project's docs directory

This will copy the contents of the docs directory from Github to the current folder - ideal if there is an existing project and you want to add to _Docsify_ it.

1. Ensure you have `curl` command installed. Or use `wget`.
2. Navigate to your project's `docs` folder.
    ```sh
    cd my-project/docs
    ```
3. Download necessary files in the template [docs](/docs) directory to your project using this two-line command. (The `-O` flag will save the files locally, keeping the original filenames.)
    ```sh
    REPO_DOCS='https://raw.githubusercontent.com/abpanic/docsify-template/master/docs/'
    curl $REPO_DOCS\{_coverpage.md,_sidebar.md,.nojekyll,index.html,README.md\} -O
    ```

### Customize

You can use your IDE to do find and replace across files.

Use the convenient [replace.sh](/replace.sh) script in this repo to replace the template's values with your own.


1. Find the script.
    - If you used the template button, you've already got it.
    - If adding content to your existing project's docs, copy script to your project **root** (not docs directory)
        ```sh
        curl 'https://raw.githubusercontent.com/abpanic/docsify-template/master/replace.sh' -O
        chmod +x ./replace.sh
        ```
2. Modify the `MY_` values then run this script to replace the template's value with your own.
3. Run the script from the **project root** against yours docs directory.
   ```sh
   ./replace.sh
   ```
4. The script can be deleted after you use it.

Now complete any remaining TODO items in the files.

### Use template readme

If you clicked _Use this template_, followed the customize steps above, then the last thing to do is replace the project's README.md file with the template one.

```sh
mv README.template.md README.md
```

Then customize README.md as your own project.


## Set up and run

### Remote use

Whatever approach you use to set up a `docs` directory, you can use your own project or a forked template and serve your site on platform like  GiHhub Pages or Netlify.

This template still works fine as a standalone online demo of _Docsify_ that you can tweak. In a real project, you'd add your code at the repo root, outside of `docs`. Or you could move your docs site to the repo root on the `gh-pages` branch for GH Pages.

### Serve locally

Follow this [gist](https://gist.github.com/abpanic/1e5ef827664de555a7affe9702864287) so you can view the docs site on a local webserver.

Go to my [DocsifyJS Tutorial - Serve locally](https://learn-docsify.netlify.app/#/?id=serve-a-docsify-site-locally) for more info on what DocsifyJS is and how to use it.


## Related projects

A template using Docsify Themeable. It is a Docsify site but easier to use, it is prettier (in my opinion), and supports a theme system that is more advanced than that in Docsify.

- [![Docsify-themeable-quickstart](https://img.shields.io/static/v1?label=abpanic&message=docsify-themeable-quickstart&color=blue&logo=github)](https://github.com/abpanic/docsify-themeable-quickstart)

A template for Vue-based docs site. Except it uses VuePress to render a static site (better for SEO) rather than as a Single-Page Application like Docsify.
 
- [![Vuepress-quickstart](https://img.shields.io/static/v1?label=abpanic&message=vuepress-quickstart&color=blue&logo=github)](https://github.com/abpanic/vuepress-quickstart)

A template for a Vue-based app.

- [![Vue-quickstart](https://img.shields.io/static/v1?label=abpanic&message=vue-quickstart&color=blue&logo=github)](https://github.com/abpanic/vue-quickstart)


## License

Released under [Unlicense](/LICENSE) by [@Abhilash](https://github.com/abpanic).

- You can modify and reuse this project.
- Please link back to the original repo somewhere in your project if you use this in any way.
- Including an original license copy.
    - If you add content from [docs](/docs/) to your repo (or click _Use this template_) and then modify for your own needs so your copy is no longer a template, then you don't need to include a license.
    - If you do fork this repo then use it as your own _template_, then this project's license and copyright notice must be **included** with the software. [source](https://choosealicense.com/licenses/#mit). Copy `LICENSE` to `LICENSE-source` and then update your copy of `LICENSE` with your own details.
