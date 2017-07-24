# `ghc-dlas` - GHC 8 Tarballs without large address space

Provides binary Ubuntu 14.04 LTS tarballs for GHC distributions, configured with `--disable-large-address-space`. 

This is useful, because WSL (Windows Subsystem for Linux) doesn't cope well with GHC 8's scheme of reserving a huge chunk of virtual memory (yet).

You can then use these together with e.g. `stack` in the way outlined by [Vincent Hanquez](https://vincenthz.github.io/posts/haskell/2017-07-20-ghc-stack.html), maybe even create your own custom snapshots (will need a recent `stack`, which you have to compile yourself for the same reasons) and enjoy Haskell development in your favorite Windows development environment.

Of course, this should only be temporary, as the WSL team [seems to be on it](https://github.com/Microsoft/BashOnWindows/issues/1671).
