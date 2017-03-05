---
layout: page
title: CI/CD portfolio
---

# CI/CD portfolio

## Migration from Bash to Ruby scripts

When I joined one of my employers, we were using bash scripts in order to build
iOS and Android projects, as well as signing it and uploading to HockeyApp.

Over time, we migrated to Ruby those scripts so as to have proper arguments in
the script (--hockey-app-token Token instead of relying on order), and to maintain
our scripts in a language the company had experience on (after using Calabash for
automation testing).

On top of that migration, we included in the script toolbox:

* Generate version number from git hash, plus build metadata (e.g. environment built for).
* Tweak XCArchives before signing them to configure build flavours without requiring a full rebuild (saves compilation time).

## Migration from Ruby scripts to Fastlane generic script

After undertaking the first migration, we decided to give Fastlane a go. Since the
company is an agency, we had to cater for several projects that behave mostly the same,
so I took charge of writing a generic Fastlane Fastfile that would later be tweaked
from a YAML configuration file containing metadata specific to the project.

This approach was later adopted by the London office, and is currently being considered
to be used globally (though different practices amongst different offices hinder this).

This migration involved:

* Writing Fastlane actions wrapping the initial Ruby scripts we had.
* Writing a Fastfile to cover all the different kind of jobs we have in all the projects.
* Designing the configuration YAML file.
* Documenting it all. If it is not documented, it doesn't exist.
* Creation of sample project using this new approach.

With this, other projects would import as a submodule the Fastlane repository and
edit the sample YAML file contained, and then they could run in Jenkins commands like:

* fastlane ci
* fastlane daily
* fastlane release
* ...

A benefit of this approach is that the repository contains the description on how
to build itself by pointing to the fastlane wrapper repository and containing the
YAML configuration file, so builds are more reproducible in any machine rather than
just in Jenkins as they were previously, where reproducing a build was this tedious
task of replaying the commands Jenkins used.
