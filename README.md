# heroku-buildpack-qgsocksify

**:warning: This is an unofficial Heroku Buildpack.**

Heroku Buildpack to install [qgsocksify](https://devcenter.heroku.com/articles/quotaguardstatic#installing-the-quotaguard-static-socksify-wrapper)

`qgsocksify` is the QuotaGuard Static socksify wrapper. It's related to [Heroku Add-on QuotaGuard Static](https://devcenter.heroku.com/articles/quotaguardstatic).

## How it works

Installs from official [qgsocksify binary](https://s3.amazonaws.com/quotaguard/quotaguard-socksify-latest.tar.gz) on Amazon S3.

`qgsocksify` installation ends in `/app/bin` directory.

## Configure from CLI

```
$ heroku buildpacks:add https://github.com/feedforce/heroku-buildpack-qgsocksify.git
```

## Configure from app manifest

```json
{
  "buildpacks": [
    {
      "url": "https://github.com/feedforce/heroku-buildpack-qgsocksify.git"
    }
  ]
}
```

## License

MIT © [Feedforce Inc.](https://github.com/feedforce)
