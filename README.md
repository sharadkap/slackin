# slackin

Deploy [`slackin`](https://github.com/rauchg/slackin) to [Now](https://now.sh)!

Deploying slackin directly (`now rauchg/slackin …`) works just fine,
however there is a `gulp` build process that every deployment has to do
in that case.

The [`slackin` package](https://npmjs.org/slackin) in the npm registry has
the build files pre-compiled with the package, so when you
`npm install slackin` you don't have to build locally, so that's what this
repository does.

There's only the single [`package.json` file](./package.json), so be sure to
read it to understand what's going on!

## How to deploy

First, [download `now`](https://zeit.co/download). Then, run the following command:

```
$ now -e SLACK_API_TOKEN="<token>" -e SLACK_SUBDOMAIN="<team-name>" now-examples/slackin
```

## License

MIT
