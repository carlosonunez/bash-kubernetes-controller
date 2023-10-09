# bash-kubernetes-controller

A Kubernetes controller written in pure Bash.

## What does it do?

It's a really dumb controller. It:

- Prints this log on `Pod` startup:

  ```text
  A new `Pod` appeared! $INFO_ABOUT_POD
  ```
- Prints this log on `Pod` shutdown:

  ```text
  Pod `$POD_NAME` had enough and quit.
  ```

`bash-kubernetes-controller` will only print these logs for `Pod`s
that have `apps.carlosnunez.me/witness-me-exclamation-mark` set to `true`.

## But why?!

I wanted to understand how Kubernetes controllers work top-down.

The only way I can understand things with this many moving parts is through
lots of concentrated suffering.

So here we are.

## How To Use

More to come.

## But, yeah, don't use this

This project accompanies a series of blog posts I wrote on understanding
Kubernetes controller. It is not, and never will be, meant for production use.

Want to write your own for-real controller?
[Check this out](https://scribe.rip/geekculture/kubernetes-custom-controller-6bb29a859dc)

Want to turn a Bash script into an operator?
[Check this out instead](https://github.com/flant/shell-operator)
