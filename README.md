## Rock Paper Scissors! ##
Implements rock paper scissors in a small web app.

#### Setup #### 

Check that you have ruby installed

`ruby -v`

If not, install instructions can be found [here](https://www.ruby-lang.org/en/documentation/installation/).

Clone the repo on the command line by running

`git clone git@github.com/Le5tes/rps-challenge.git`

Check that you have bundler installed

`bundler -v`

If not, install by running

`gem install bundler`

Install dependencies by running

`bundle`

Run using 'rackup' or 'ruby app.rb'.
Play by entering your name on the homepage, then clicking on the picture of the rock, paper or scissors.

### Context ###
This was one of the earlier challnges at MakersAcademy. We were given a weekend to write a web app for playing rock, paper scissors against the computer.

### Approach ###
The app and routes are built using sinatra. 
The game itself is contained within the Game model. When the game is run, the app accesses the game class instance variable which is set to an instance of the game.
My approach towards the game logic was to use a data table and look up the wins and loses. This is both neat and easily scalable.
The player class is quite basic, and allows players to make choices. Currently the Computer playing logic is kept within the game- it may make more sense to move this either into the player class or better to make a new computer-player class that is polymorphic with player. 
