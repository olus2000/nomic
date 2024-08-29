================================================================================
                          Web Nomic Hosted by olus2000
================================================================================

**THIS IS A DRAFT OF AN IDEA**

There's a Host. The Host can play the game but can't win it. The Host oversees
the game and has the final say in every dispute. The Host should avoid
interfering with the game unless it is important for the game to continue.

The game is played on a combination of a git repository and a web server, both
of which should be publically accessible. The Host should have control over both
the repository and the server, but access to the repository should be open for
cloning in case a host change is desired. The git repository contains a web
application that is accessible through the web server and which is part of the
game.

This is a Nomic, a game about changing rules. It is played by making pull
requests to the repository which will affect the app running on the web server,
as well as any additional game mechanics implemented in the app in the process.
Every pull request should be subject to a vote and can be vetoed at will by the
Host if it is suspected that it could compromise integrity of the server.

Because it's a Nomic it has a set of rules. They are listed in this document,
but when the game actually starts they should be displayed in the web app
instead. The players are responsible for adhering to these rules and may include
consequences for breaking them. The Host should oversee that the rules are being
followed, especially when it comes to pull requests. It is recommended that a
change to the rules comes with a change to the web app functionality that
reflects that rule change.
