# Setup Clojure Kitchen Sink

> This does NOT currently work due to limitations of composite actions.
> See https://github.com/actions/runner/issues/646 for more information.

This is a kitchen sink of various Clojure(Script) dependencies.
I'll continue to extend the action as there's more dependencies
I use in my projects. The action currently installs the following:

- `node.js`
- `java`
- `clojure`
- `babashka`

Additionally, it will clone your repo and setup the container
to use a GitHub PAT (so that you can install private packages).

### Inputs

| Input             | Description                                                    |
|-------------------|----------------------------------------------------------------|
| `github-token`    | A personal access token (PAT) used to pull down private repos. |
| `github-username` | The username that the PAT is associated with.                  |
