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


--------------------------------------------------------------------------------
                                     Rules
--------------------------------------------------------------------------------

The game's rules are divided into two parts: the Host rules, and the player
rules. The former are meant to define the rough structure of the game and ensure
safety for the Host's server, while the latter are the object of the game, to be
shaped by the will of the players.


Host rules
==========

0. The Host rules can only be changed by a Host.

1. At least one person chooses to be the Host of the game at its start.

2. A Host may be a player, but may not win the game.

3. Any Host may abdicate at any point, but the game cannot progress without a
   Host.

4. With a unianimous decision of all Hosts a new Host may join at any point.

5. The Hosts are responsible for maintaining a repository.

   a. The repository shall be accessible to all players for reading.

   b. The repository shall be accessible to all Hosts for reading and writing.

6. The Hosts are responsible for maintaining a web server.

   a. The server shall be accessible to all players.

7. The repository defines a web application which shall be hosted on the web
   server.

   a. The web application shall include the whole set of rules of the game in a
      way that is accessible to all players and Hosts.

8. All changes to the rules of the game shall be implemented via change
   proposals to the repository.

9. Any Host may reject any change proposal.

10. Any Host may implement any change to the repository at any point without any
    prior consultation.

11. Any Host may remove any non-Host player from the game at any point.

12. Any Host may forbid any non-Host non-player from joining the game.

    a. Non-players may not join the game unless all Hosts who have forbidden
       them from doing so agree.

99. In case of conflict of rules:

    a. A decision by any Host takes priority over any rules until the conflict
       is resolved.

    a. The Host rules take priority over other rules, but not over Host
       decisions from rule 99a.


Player rules
============

100. Any player may willingly drop out of the game at any point.

101. Any non-player that wasn't in the game for at least 24h can get invited
     into the game by any player.

     a. If the invitation is accepted they join the game as a player.

102. The game is held in the github repository ``nomic`` owned by ``olus2000``
     and on the website ``olus2000.pl``

     a. Link to the repository: https://github.com/olus2000/nomic

     b. Link to the website: https://olus2000.pl/nomic

103. Every player can create one change proposal.

     a. After the proposal has been implemented or rejected its creator may
        create a new one.

     b. Any player may replace their proposal with a new one at any time.

     c. The proposals take the form of github pull requests to the repository.

104. Every player can vote on every proposal.

     a. Voting is performed by reacting to the first post in the github pull
        request with either "thumbs up" or "thumbs down" emoji, indicating
        approval or disapproval respectively.

     b. Proposals that get approval of over 50% of players should be implemented
        by the Hosts.

     c. Proposals that get disapproval of at least 50% of players should be
        rejected by the Hosts.

105. When a proposal has been implemented its creator gets awarded 1 point.

     a. Current standings can be seen on the website.

106. First player to reach 20 points wins the game.

107. The game ends when a player wins it.
