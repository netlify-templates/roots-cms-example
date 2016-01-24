# Roots + netlify CMS

This is a simple example of how to integrate netlify CMS with a roots based site.

It's based on Brian Rinaldi's great [Static Site Samples](https://github.com/remotesynth/Static-Site-Samples) and meant as a simple example of how to hook netlify CMS up with a roots based site.

## Setting up

Make sure to install the [netlify-git-api](https://github.com/netlify/netlify-git-api) before you start.

Then:

```bash
git clone https://github.com/netlify-templates/roots-cms-example.git
cd roots-cms-example
netlify-git-api users add
netlify-git-api serve
```

Open a separate terminal window and run:

```bash
npm install
roots watch
```

## Using

Visit [localhost:1111](http://localhost:1111/) to browser the site.

Visit [localhost:1111/admin](http://localhost:1111/admin) to use the CMS.

To run against the GitHub API in production, edit the production backend settings for `admin/config.yml` with the correct repository and branch.

Then make sure to set a `CMS_ENV` environment variable to `production` when running the production build.
