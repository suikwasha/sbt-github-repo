# a fork of sbt-github-repo

creates your own Maven/ivy repository on Github.

## Installation

Add the following to `project/plugins.sbt` or `~/.sbt/plugins/plugins.sbt` file:

    resolvers ++= Seq(
        "jgit-repo" at "http://download.eclipse.org/jgit/maven",
        "sbt-github-repo" at "http://suikwasha.github.io/sbt-github-repo"
    )

    addSbtPlugin("com.github.suikwasha" % "sbt-github-repo" % "0.1.1")

## Publishing

If you want to create a repository on `git@github.com/suikwasha/repo`

Run `sbt publish-ghrepo git@github.com/suikwasha/repo` to publish your artifacts.
plugin creates branch `gh-pages` automatically.
