# UBIRCH DOCU THEME

Theme for GitHub pages with documentational purpose of UBIRCH projects

----
Based on The [Hacker theme](https://github.com/pages-themes/hacker) - a Jekyll theme for GitHub Pages.

![Thumbnail of Hacker](thumbnail.png)

---
## Usage

To use the UBIRCH docu theme:

1. Add the following to your site's `_config.yml`:

    ```yml
    remote_theme: ubirch/ubirch-docu-theme@main
    plugins:
    - jekyll-remote-theme # add this line to the plugins list if you already have one
    ```

2. Optionally, if you'd like to preview your site on your computer, add the following to your site's `Gemfile`:


    ```ruby
    gem "ubirch-docu-theme"
    ```

Run the command `bundle install` in the root of project to install the jekyll remote theme gem as a dependancy

Run `bundle exec jekyll serve` to build and serve your site


## Customizing

### Configuration variables

UBIRCH Docu Theme will respect the following variables, if set in your site's `_config.yml`:

```yml
title: [The title of your site]
description: [A short description of your site's purpose]
```

Additionally, you may choose to set the following optional variables:

```yml
show_downloads: ["true" or "false" (unquoted) to indicate whether to provide a download URL]
google_analytics: [Your Google Analytics tracking ID]
```

### Previewing the theme locally

#### Prerequisites:

Ruby and Jekyll installed - see [Jekyll Installation Guide](https://jekyllrb.com/docs/installation/)

#### Build and Run Theme

If you'd like to preview the theme locally (for example, in the process of proposing a change):

1. Clone down the theme's repository (`git clone https://github.com/pages-themes/hacker`)
2. `cd` into the theme's directory
3. Run `script/bootstrap` to install the necessary dependencies
4. Run `bundle exec jekyll serve` to start the preview server
5. Visit [`localhost:4000`](http://localhost:4000) in your browser to preview the theme

### Running tests

The theme contains a minimal test suite, to ensure a site with the theme would build successfully. To run the tests, simply run `script/cibuild`. You'll need to run `script/bootstrap` once before the test script will work.
