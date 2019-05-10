# How to reproduce

1. `git clone https://github.com/yeputons/cabal-type-class-default-impl-rebuild.git`
1. `cabal v1-test` or `cabal new-test`
1. Ensure that tests fail
1. Update `src/MyClass.hs` by commenting the line with `undefined` and uncommenting the line with `10`
1. `cabal v1-test` or `cabal new-test`
1. Ensure that tests still fail
1. `cabal v1-clean` or `cabal new-clean`
1. `cabal v1-test` or `cabal new-test`
1. Ensure that tests now pass
