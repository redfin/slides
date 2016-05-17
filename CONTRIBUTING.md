To add a new presentation using [reveal.js](http://lab.hakim.se/reveal-js/)

- Clone the reveal.js repository somewhere (we'll use `~/code/presentations`)
- Clone the slides repository somewhere (we'll use `~/code/slides`)
- Create a new subdirectory in the slides repository `mkdir ~/code/slides/my-awesome-presentation`
- Move the generated source `cp -r ~/code/presentations ~/code/slides/my-awesome-presentation`
- Add the [custom Redfin theme](/python-at-redfin/css/theme/redfin.css) by copying the theme into your css/theme directory, and changing the theme style tag's href to `css/theme/redfin.css`
- Develop your presentation locally (`npm i && npm start` then hack in watch mode)
- Create a new commit on the gh-pages branch of slides
- Push to the slides repository
- See your sweet new slides at https://redfin.github.io/slides/my-awesome-presentation
- Add a small blog post to [the engineering blog](https://www.redfin.com/blog/category/redfin-ceo/engineering-at-redfin) with a link to your new presentation
- Add a link to your new presentation to [index.html](/index.html)

Remember, its just a static site, so you can use any web technology you can think of, reveal is just one option.

If you commonly forget that the main development branch is called `gh-pages` instead of `master`, you can create an alias

    git symbolic-ref refs/heads/master refs/heads/gh-pages
