# Why fork this repo?

To have hermetic/reproducible builds, we need to not only be able to
check out a specific hash of the repo, but also track the dependencies
that the tools are built with and use, at build time. Given the
current state of the `dep` build tool (currently 0.4.1), this means we
have to track the deps for this project seperately.

# Usage & Updating

We're not actually changing anything, just adding Gopkg.lock &
Gopkg.toml files. As such, using and updating the package can be a bit
of a pain. You have to check the repo out into a $GOPATH under
src/github.com/golang/protobuf dir and work from there.

