# Release Manifests

## What is this?

This directory contains the repo manifests used to build a particular Mendel
release. Each time an image is made from Jenkins, the resulting manifest
snapshot is placed here to allow for reproducing the build on another machine.

## How do I use this?

To make an earlier build with these manifests, simply copy the manifest you need
out of this tree into your `$ROOTDIR/.repo/manifest.xml` and call `repo sync` to
bring your tree up to date with those commits.

The general format of the paths are `$BOARDNAME/$RELEASENAME-$RELEASEVER.xml`,
so to find the eagle 5.0 release for enterprise, you'd want to use the
`enterprise/eagle-5.0.xml` release.
