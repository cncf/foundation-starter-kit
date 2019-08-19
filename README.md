# The Foundation Starter Kit

Are you starting a new OSS foundation under the [Linux Foundation](https://linuxfoundation.org) or [Cloud Native Computing Foundation](https://cncf.io)? Or even under a different organizational umbrella? This repo provides a starter kit that enables you to get up and running quickly on building a site.

## Getting started

In order to use this kit, you'll need to have the following installed:

* The [Yarn](https://yarnpkg.com/en/) dependency management tool. Installation instructions are [here](https://yarnpkg.com/en/docs/install#mac-stable).
* The [Hugo](https://gohugo.io) static site generator. Installation instructions are [here](https://gohugo.io/getting-started/installing/); make sure to install the "extended" version.


Once you have those tools installed, clone the repo and `cd` into the directory:

```bash
git clone https://github.com/cncf/foundation-starter-kit
cd foundation-starter-kit
```

Install the necessary assets:

```bash
make setup
```

Now you can run the site locally:

```bash
make serve
```

Open your browser to `http://localhost:1313` and you'll see a generic version of the site.

## Customizing

### Configuration

There's a wide variety of variables that you can update in the [site config](./config.toml).

Parameter | Description
:---------|:-----------
`params.colors` | The site's basic color palette
`params.font_awesome_version` | The version of [Font Awesome](https://fontawesome.com/) used for the site's icons
`params.description` | A short, pithy description of your foundation
`params.copyright` | Copyright text for the foundation
`params.github_repo` | The [GitHub](https://github.com) repo associated with the foundation (if any)
`params.info` | Various bits of informational text for the site's front page
`params.explanation` | More informational text for the site's front page
`params.fonts` | The font used for the site. Must be available via [Google Fonts](https://fonts.google.com).
`menu.main` | Text and links for the main menu of the site (displayed in the site's navbar)

### Members

You can specify the member organizations—for-profit companies, non-profit orgs, etc.—in [`data/members.yaml`](./data/members.yaml). You can specify a URL for the member org as well as filename for the org's image. That image needs to be added to the [`static/img/logos/members`](./static/img/logos/members) directory.

**Example**: https://foundation-starter-kit.netlify.com/members

### About

Update the foundation's "About" page in [`content/about.md`](./content/about.md).

### News

You can create news articles by adding Markdown files to the [`content/news`](./content/news) directory. Each news article must have the following metadata:

* `title`
* `author`
* `date` (in `YYYY-MM-DD` form)
* `layout` (must be set to `news-item`)
