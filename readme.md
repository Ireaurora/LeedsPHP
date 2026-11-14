# LeedsPHP

LeedsPHP's website is built with [Jekyll](https://jekyllrb.com).

## Run locally with Docker

Install and start Docker Desktop, then run the command for your terminal from
the repository root.

### macOS or Linux

```
docker run --rm \
  --volume="$PWD:/srv/jekyll" \
  --volume="$PWD/vendor/bundle:/usr/local/bundle" \
  --env JEKYLL_ENV=development \
  -p 4000:4000 \
  jekyll/jekyll:3.8 jekyll serve
```

### Windows (PowerShell)

```powershell
docker run --rm `
  -v "${PWD}:/srv/jekyll" `
  -v "${PWD}\vendor\bundle:/usr/local/bundle" `
  --env JEKYLL_ENV=development `
  -p 4000:4000 `
  jekyll/jekyll:3.8 jekyll serve --host 0.0.0.0
```

Open <http://localhost:4000>.

## Run without Docker

Install Ruby and Bundler, then run these commands from the repository root:

```sh
bundle install
bundle exec jekyll serve
```
