# ShowFolio theme for Hugo

![Latest Release](https://img.shields.io/github/tag/apvarun/showfolio-hugo-theme.svg)
![ShowFolio hugo theme](https://img.shields.io/github/license/apvarun/showfolio-hugo-theme)
![Hugo generator](https://img.shields.io/badge/generator-hugo-brightgreen)

ShowFolio is a modern portfolio theme for your Hugo site.

![Preview](https://github.com/apvarun/showfolio-hugo-theme/raw/main/images/showfolio-dark.png)

**Features:**

- Responsive content
- Codepen Embeds
- Blog
- Social links
- Dark mode

➡️ [DEMO](https://showfolio.vercel.app/)

## Get the theme

Minimum Hugo Version: 0.69.0

Run from the root of your Hugo site:

```sh
git clone https://github.com/apvarun/showfolio-hugo-theme.git themes/showfolio
```

Alternatively, you can include this repository as a [git submodule](https://git-scm.com/docs/gitsubmodules). This makes it easier to update this theme if you have your Hugo site in git as well:

```sh
git submodule add https://github.com/apvarun/showfolio-hugo-theme.git themes/showfolio
```

## Setting up the theme

- Install postcss-cli globally using `npm install -g postcss-cli`
- Copy package.json to the root folder of your website and run `npm install`
- Finally run `hugo serve`

## Preview the theme

ShowFolio theme ships with an fully configured example site. For a quick preview:

```sh
cd themes/showfolio/exampleSite/
hugo serve --themesDir ../..
```

Then visit `http://localhost:1313/` in your browser to view the example site.

## Configuring theme to a hugo website

1. Copy `package.json` and `package-lock.json` to the root folder of your the website
2. Run `npm install` to install required packages for theme
3. Run `npm i -g postcss-cli` to use PostCSS with Hugo build
4. Set `theme = 'showfolio'` in config.toml
5. Run `npm start` to start your local server

Make sure to commit the above changes to your repository.

When deploying to services like Netlify or Vercel, use the following command for building your site:

```sh
npm i && hugo -D --gc
```

## Add content

The following explains how to add content to your Hugo site. You can find sample content in the `exampleSite/` folder.

### Structure:

    .
    ├── ...
    ├── blog       # Blog Section
    │   ├── post1   # Post 1
    │   ├── post2   # Post 2
    │   └── _index     
    └── ...

## Configure your site

From `exampleSite/`, copy `config.toml` to the root folder of your Hugo site and change the fields as you like. Helpful comments are provided.

## Menu

Menu in ShowFolio theme is pre-set to have blog and about pages.

## Google Analytics

Set `googleAnalytics` in `config.toml` to activate Hugo's [internal Google Analytics template](https://gohugo.io/templates/internal/#google-analytics).

## Issues

If you have a question, please [open an issue](https://github.com/apvarun/showfolio-hugo-theme/issues) for help and to help those who come after you. The more information you can provide, the better!

## Contributing

Contributions are welcome. For major changes, please open an issue first to discuss what you would like to change.

## License

Licensed under [MIT](LICENSE)
