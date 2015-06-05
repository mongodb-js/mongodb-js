# Quality

> @wip: Actively collecting feedback from contributors to create a set of shared
> best practices. The result of this will be incorporated into a
> tooling module ([mj](https://github.com/mongodb-js/mj)) which will automate
> as much of the process as possible.

## Testing

- `<required>`: `npm test` returns a non-zero exit code
- `<required>`: TravisCI connected to your project
- `<required>`: CI configured to test against your project's appropriate [supported environments](#supported-environments)

## Code Coverage

- `[optional]`: If it's easy for your project then do it, else don't sweat it.

## Style

- `<required>`: `npm run check` returns a non-zero exit code
- `[optional]`: Your check script lints, formats and smoke tests your project

## Versioning

- `<required>`: Use responsible semver so you don't break your upstream dependencies
- `[optional]`: Make major version releases whenever possible

## Supported Environments

### `.travis.yml`

```yaml
os: linux
language: node_js
# node.js support: Latest stable version, `0.10.x`, and `0.8.x`
# iojs support: Latest stable version
node_js:
  - "node"
  - "0.10"
  - "0.8"
  - "iojs"
# MongoDB Support: Latest 2.6, Latest 3.0 and Latest unstable
# @see https://github.com/mongodb-js/version-manager/blob/master/README.md#travisci-automation
env:
  - MONGODB_VERSION=2.6.x
  - MONGODB_VERSION=3.0.x
  - MONGODB_VERSION=3.1.x
```

### `appveyor.yml`

```yaml
# @todo: Figure out which versions of windows this will actually build node-pre-gyp bins for.
# windows arch support: 32-bit and 64-bit
# node.js support: Latest stable version, `0.10.x`
# iojs support: Latest stable version
environment:
  matrix:
    - nodejs_version: 0.10.36
      platform: x86
      msvs_toolset: 12
    - nodejs_version: 0.10.36
      platform: x64
      msvs_toolset: 12
    - nodejs_version: 0.12.0
      platform: x86
      msvs_toolset: 12
    - nodejs_version: 0.12.0
      platform: x64
      msvs_toolset: 12
    - nodejs_version: 1.1.0
      platform: x86
      msvs_toolset: 12
    - nodejs_version: 1.1.0
      platform: x64
      msvs_toolset: 12
```

### `.zuul.yml`

```yaml
# We will make sure all modules usable in the UI work with the following browser versions.
browsers:
  - name: chrome
    version: latest
  - name: safari
    version: latest
  - name: firefox
    version: latest
  - name: ie
    version: latest
  - name: iphone
    version: latest
```

## Documentation

- `<required>` A `README.md` file.
- `<required>` `README.md` contains at least 1 example of how to use your module or a `View Examples` link.
- `<required>` Use jsdoc tags for at least `exports` of your main module.

### FAQ

#### "Why should I care about docs?  I want to write features!"

Nobody will use your project if it doesn't look like they can trust it.  Fear not the days of `jsdoc`
generating hundreds of html files with 0 content.  [mj](http://github.com/mongodb-js/mj) will
  - provide a nice shared theme
  - use [dox](http://npm.im/dox) to build your docs content (for example, [connect-mongodb-session](http://github.com/mongodb-js/connect-mongodb-session))
  - publish a pretty version to your projects github page as a part of [releasing][#releasing]

## Releasing

- Must have a `.npmignore` file so at least your project's tests/examples/docs are excluded from the tarball published to npm
- Binary add-ons should use [node-pre-gyp](https://github.com/mapbox/node-pre-gyp)
- [mj](https://github.com/mongodb-js/mj) will provide the following for all modules:
  - no humans required
  - publish to npm
  - publish notification to a REST endpoint (shows up in flockdock/gitter activity feeds)

## Code Review

- Do it.
- Use pull requests
- [reviewable.io](http://reviewable.io) is nice, easy, free and integrates very well with github
- Get feedback from users and create a context trail for your fellow and future contributors

## Contributor Guidelines

- `<required>` A `CONTRIBUTING.md` file
- @todo: What are some good examples we could use to add to templates?

## Licensing

- `<required>` A `LICENSE` file
- `<required>` Apache License 2.0
- `<required>` The `license` of your project's `package.json` must not be empty.

### FAQ
#### Why Apache License 2.0?

It's what we use for all of the drivers already and is very permissive. It differs from the MIT
license by clarifying several key details, including patent and trademark rights.

#### Why is this part of quality?

Licensing audits are part of the process for start-up financing (technical due dilligence) and bringing projects into the enterprise (get sign-off from legal).  This is a painful process we must make as simple as we can.  For more details, see [davglass/license-checker](https://github.com/davglass/license-checker).
