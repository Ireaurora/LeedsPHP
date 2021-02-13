# LeedsPHP

This site runs on [jekyll](http://jekyllrb.com).

To make it run locally: `bundle exec jekyll serve`

# Install

To make life easy for yourself, just use Docker so you don't have to spend a few hours messing about with Ruby and Gem versions. 

The following line will run jekyll serve via Docker. 

```
docker run --rm --volume="$PWD:/srv/jekyll" --volume="$PWD/vendor/bundle:/usr/local/bundle" --env JEKYLL_ENV=development -p 4000:4000 jekyll/jekyll:3.8 jekyll serve
```


