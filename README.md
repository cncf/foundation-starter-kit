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

Now you can run the site locally:

```bash
make serve
```

Open your browser to `http://localhost:1313` and you'll see a generic version of the site.