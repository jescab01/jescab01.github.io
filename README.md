

A quicker, cleaner way to get started blogging with a template version
of Jeckyll. In this case, [al-folio](https://github.com/alshedivat/al-folio/blob/main/INSTALL.md).

# Installation

1. Install Ruby - https://www.ruby-lang.org/en/downloads/; Installing **MSYS2** is also needed.
2. Install Ruby gems - https://rubygems.org/pages/download/
3. Install Jekyll and Hydejack: > gem install jekyll jekyll-theme-hydejack

# Running locally
1. Clone repository (git users), or [download] and unzip.
2. Open terminal, `cd` into root directory (where `_config.yml` is located)
3. Run `bundle install` [^1]
4. Run `bundle exec jekyll serve`
5. Open <http://localhost:4000/>


----


# Editing the site

Go to [CUSTOMIZE.md](CUSTOMIZE.md) or read it on the [github site](https://github.com/alshedivat/al-folio/blob/main/CUSTOMIZE.md)


## Inset figures in Markdown

Two approaches, the first one may be more efficient, so the reader can have a quick look on the static 
figures before clicking on them and going to a slower loading of the dynamic figures.

1) opening the figure in another window.
[<img src="/research/th/icon_th.png">](/research/th/figs/Criticality_th_noisy_phetero.html)

2) inserting the figure in the same page.
<iframe width="100%" height="400"
  src="/research/th/figs/Criticality_th_noisy_phetero.html"
  frameborder="0" allow="autoplay; encrypted-media"
  allowfullscreen></iframe>


# Publish it
Just do a commit to github, easy enough.
