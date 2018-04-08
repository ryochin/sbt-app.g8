README
======

A simple but complete "Hello World Starter Kit" for Scala 2.12.

* appropriate options
* auto formatting
* specs2
* native-packager
* typesafe-config
* scala-logging

Setup Java
----------

go to https://www.java.com/en/download/ and install Java8.

Setup Scala
-----------

### OSX

	brew install scala sbt

Usage
-----

	sbt new ryochin/sbt-app.g8
	cd my-app

	vi src/main/scala/Main.scala

	sbt compile
	sbt test
	sbt run

	curl -L -o .gitignore https://github.com/github/gitignore/raw/master/Scala.gitignore
	git init
	git add .
	git commit -m "initial import."

	sbt stage
	target/universal/stage/bin/my-app -main Main

### by Makefile

	make compile
	make test
	make run
	make run-app            # stage and run
	make run-app-command    # run only
	make doc                # open html
