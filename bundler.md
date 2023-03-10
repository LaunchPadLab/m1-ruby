# Bundler post-install

Because Bundler versioning is a pain, their Docs point us in the direction of getting the right version installed:

```
gem install bundler -v "$(grep -A 1 "BUNDLED WITH" Gemfile.lock | tail -n 1)"
```

Solution originally sourced from here: https://bundler.io/blog/2019/05/14/solutions-for-cant-find-gem-bundler-with-executable-bundle.html

#### Verified by:
- [Lanny Bose](https://github.com/LannyBose) on an M1 MacBook Pro on MacOS 12.6.1