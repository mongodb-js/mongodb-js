# Daily Things to Know

## Committing/Branching/Naming

For small ("micro-")modules, it's okay to just have a single _master_ branch.

For anything larger (like apps, or complex modules) we're loosely following
[nvie's branching model](http://nvie.com/posts/a-successful-git-branching-model/),
where _master_ is the stable branch, _develop_ (or _dev_) is bleeding edge,
and bufixes and features live on feature branches until they are reviewed and
merged into the develop branch. nvie's release and hotfix branches are not
that important (at least not yet).

In any case, please read the `CONTRIBUTING` document in the repo's root
directory for specific instructions how to contribute.

If you send a pull request, please also check what branches exist on the
target repo. If there is more than one branch, then you should probably not
send pull requests to _master_.

> @todo: continue naming scheme mongodb-{functionality}?

## Profiling & Debugging

- [traceviewify](http://thlorenz.github.io/traceviewify/) Converts .cpuprofile
  format to trace viewer JSON object format to allow analysing the data in `chrome://tracing`
- [node-inspector](https://www.npmjs.com/package/node-inspector)  debugger
  interface for Node.js applications that uses the Blink Developer
  Tools (formerly WebKit Web Inspector).
- [look](https://github.com/baryshev/look) Performance profiler based
  on [nodetime](https://nodetime.com/)
- [automated-chrome-profiling](https://github.com/paulirish/automated-chrome-profiling)
  use `chrome-remote-interface` instead of manually opening files in chrome.
