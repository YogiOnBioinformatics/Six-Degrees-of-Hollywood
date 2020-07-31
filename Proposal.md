## 1520 Project Proposal

### Overview

Our goal is to create a web-based game inspired by the parlor game [Six Degrees of Kevin Bacon](https://en.wikipedia.org/wiki/Six_Degrees_of_Kevin_Bacon) which is a game based on the theory of six degrees of separation. The idea of six degrees of separation suggests that any given person is only six or fewer social connections away from any other person. Our game will challenge the user to navigate from one actor to another using other actors and common movie appearances. Consider the following example where the user is given the starting actor and the goal.

__Start:__ Will Ferrell || __Goal:__ Michael Keaton

	{Will Ferrell}-->|Anchorman|-->{Christina Applegate}-->|Mars Attacks!|-->{Danny DeVito}-->|Batman Returns|-->{Micheal Keaton}

The above solution could be spoken; “Will Ferrell was in Anchorman with Christina Applegate. Christina Applegate was in Mars Attacks! with Danny DeVito. Danny DeVito was in Batman Returns with Michael Keaton.” The above solution would be a valid solution but may not be the shortest solution. 
	
As illustrated above, the network can best be visualized as a graph where each vertex is an actor and the set of edges connected to that vertex will be the set of all movies in which that actor has appeared.

### Plan

TMDb (The Movie Database) offers free access to their API when you create an account. After a bit of research, we’ve determined that TMDb will be more than sufficient for our needs. We will be able to request information from TMDb such as movie casts, actor photos, and movie posters through their API.

Game play could start by having the user choose a starting actor. The program could then generate a random path and provide the user with the actor at the end of the path (goal actor). Game play would progress by the user filling in a text box with the name of a movie and another text box with an actor’s name who appeared in that movie with the actor from the previous step. At this point, a request to TMDb would be made to acquire the cast of the movie which was entered. The program will verify that both actors appear on the cast list. If the move is valid, actor photos and the movie poster will be requested from TMDb and displayed somewhere on screen to indicate that the player made a valid move. The game will continue in this way until the goal is achieved. 

We envision some features for this game once a working MVP has been established. These features include racing to a solution against an opponent, racing against a countdown, finding the shortest path to a solution, and having varying degrees of difficulty.

__Milestone 1:__ 
* Complete vision of MVP
* Landing page for our game
* Game instructions with example on landing page
* TMDb account

__Milestone 2:__
* Skeletal structure of site
* Ability to retrieve applicable data from TMDb
* Demonstrate ability to acquire data from TMDb with some simple feature on our landing page
* Working MVP with minimal front-end design

__Milestone 3:__ 
* Correct any bugs
* Front-end design
* Add features and functionality

__Links:__
* [Youtube tutorial that I found extremely helpful](https://www.youtube.com/watch?v=zRwy8gtgJ1A)
* [BootstrapCDN](https://www.bootstrapcdn.com/)
* [Bootstrap Templates](https://getbootstrap.com/docs/4.3/examples/)

**Delivery of fully functional, polished product!**


Daniel Cowan ||
Jerry Han ||
Connor Jordan ||
Yogi Raghav
