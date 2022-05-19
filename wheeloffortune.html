<html>
    <head>
        <title>Wheel of Fortune</title>
        <script>
            var player0;
            var player1;
            var player2;
            var playerTotalScore = [0,0,0];
            var playerCurrentScore = [0,0,0];
            var players = [];
            var playerTurn = -1;
            var things = ["rock", "ladder", "house", "lawnmower"];
            var jobs = ["police", "teacher", "electrician", "plumber"];
            var places = ["america", "mexico", "canada", "spain"];
            var puzzle;
            
            function loadScreen(){
                var canvas = document.getElementById("myCanvas");
                var ctx = canvas.getContext("2d");
                ctx.drawImage(wheel1, 0, 0, 200, 200);
            }
            // This function starts the game!
            function start(){
                // Ask for player names.
                getNames();
                
                // Update Scoreboards.
                updateScore();
                
                // Pick first player.
                pickPlayer();
                // Show whose turn it is.
                showTurn();
                
                // Announcer Dialogue
                document.getElementById("announcer").innerHTML = "Ok, " + players[playerTurn] + ", let's play!  Push Spin Wheel to start your turn!";    

                // Pick a category and word from our choices.
                pickPuzzle();

                // Update the game board.
                updatePuzzle();

                // Hide the start button.
                document.getElementById("startButton").innerHTML = "";
            }
            
            // Pick a random category and puzzle.
            function pickPuzzle(){
                var randomCategory = Math.floor(Math.random()*3);
                var randomPuzzle = Math.floor(Math.random()*4);
                if(randomCategory == 0){
                    document.getElementById("category").innerHTML = "Category: Things";
                    puzzle = things[randomPuzzle];
                }else if(randomCategory == 1){
                    document.getElementById("category").innerHTML = "Category: Jobs";
                    puzzle = jobs[randomPuzzle];
                }else{
                    document.getElementById("category").innerHTML = "Category: Places";
                    puzzle = places[randomPuzzle];
                }                
            }
            
            // Show whose turn it is right now.
            function showTurn(){
                document.getElementById("whoTurn").innerHTML = "It is now " + players[playerTurn] + "'s turn!";
            }
            
            // Update the Scoreboards.
            function updateScore(){
                // Total Score Board
                document.getElementById("totalScore").innerHTML = "TOTAL SCORES: " + players[0] + ":" + playerTotalScore[0] + "    " + players[1] + ":" + playerTotalScore[1] + "    " + players[2] + ":" + playerTotalScore[2];
                // Current Round Score Board
                document.getElementById("roundScore").innerHTML = "CURRENT ROUND: " + players[0] + ":" + playerCurrentScore[0] + "    " + players[1] + ":" + playerCurrentScore[1] + "    " + players[2] + ":" + playerCurrentScore[2];
            }
            
            // Get names of the players.
            function getNames(){
                // Ask for player names.
                player0 = prompt("What is player 1's name?"); 
                player1 = prompt("What is player 2's name?");
                player2 = prompt("What is player 3's name");
                // Let's put them into an array. 
                players.push(player0);
                players.push(player1);
                players.push(player2);
            }
            
            
            // This randomly picks a player to start the game and updates the screen.
            function pickPlayer(){
                // Pick the first player's turn!
                var randomStart = 0;
                // Returns a random integer from 0 to 2:
                randomStart = Math.floor(Math.random() * 3);
                if(randomStart == 0){
                    playerTurn = 0;
                }else if(randomStart == 1){
                    playerTurn = 1;
                }else{
                    playerTurn = 2;
                }
            }
            
            
            

            // Decide if the letter is in the word. SUPER IMPORTANT
            // If no letter...turn is over. pick new player.
            // If letter...
            // change score
            // player gets to go again.
            // Advanced: Free Spin!  Does player automatically get a no letter redo.
            
            // Wheel of Fortune.  24 Choices using Images.  0 represents bankrupt/lose turn/free spin.  We will start with just bankrupt.
            var wheelOfFortune = [500, 750, -1, 350, 250, 600, 400, 150, 250, 400, 200, 0, 450, 150, 200, 100, 0, 200, 300, 400, 500, 100, 200, 300];
            var playerGuess = "";
            var spinResult;
            function takeTurn(){
                // Did we start the game?
                if(playerTurn == -1){
                    document.getElementById("announcer").innerHTML = "Whoa! We haven't started yet!!!";
                    return;
                }

                animateWheel();
                setTimeout(function(){spinWheel();},3400);                
                setTimeout(function(){readWheel();},3800);
                setTimeout(function(){pickLetter();}, 4200);
                   
            }
            function pickLetter(){
                // Prompt to pick a letter.
                // reset playerMatches to zero prior to guessing.
                // What if the spin is a 0?
                if(wheelOfFortune[spinResult] == 0){
                    document.getElementById("announcer").innerHTML = "Lose Turn! Too bad, " + players[playerTurn] + ".  Let's move on to the next player!"; 
                    nextPlayer();
                    return;
                }else if(wheelOfFortune[spinResult] == -1){
                    document.getElementById("announcer").innerHTML = "Bankrupt! Too bad, " + players[playerTurn] + ".  Let's move on to the next player!"; 
                    nextPlayer();
                    return;
                }
                playerMatches = 0;
                playerGuess = "";
                playerGuess = prompt("Guess a letter.");
                
                // check to see if you've already guessed that letter.
                // allow you to guess a new letter.
                var found = true;
                while(found == true){
                    found = false;
                    for(var i = 0; i < guesses.length; i++){
                        if(guesses[i] == playerGuess){
                            found = true;
                        }
                    }
                    if(found == true){
                        playerGuess = prompt("That guess has already occurred. Guess a new letter.");
                    }    
                }

                guesses.push(playerGuess);
                updatePuzzle();
                
                // Update player's score!
                if(puzzleMatches > 0){
                    playerCurrentScore[playerTurn] += puzzleMatches * wheelOfFortune[spinResult];
                    updateScore();
                    document.getElementById("announcer").innerHTML = "There are " + puzzleMatches + " " + playerGuess + ". You can Spin or Solve!"; 

                }else{
                    document.getElementById("announcer").innerHTML = "There are no " + playerGuess + ". Let's move to the next player."; 
                    nextPlayer();
                }                
            }
            function spinWheel(){
                if(wheelOfFortune[spinResult] == 0){
                    document.getElementById("wheel").innerHTML = "The Wheel is currently at Lose a Turn!";
                }else if(wheelOfFortune[spinResult] == -1){
                    document.getElementById("wheel").innerHTML = "The Wheel is currently at Bankrupt! Ouch!";
                    playerCurrentScore[playerTurn] = 0;
                }else{
                    document.getElementById("wheel").innerHTML = "The Wheel is currently at " + wheelOfFortune[spinResult];
                }
                // Let the player know the value of the spin.
                document.getElementById("announcer").innerHTML = "The wheel shows $" + wheelOfFortune[spinResult]; 
                
            }

            var wheel1 = new Image();
            wheel1.src = "https://codehs.com/uploads/5055e1083ea569e7540d91dfd38b08be";
            var wheel2 = new Image();
            wheel2.src = "https://codehs.com/uploads/9060f57f7de26aa5587f6b0a5a439cb6";
            var wheel3 = new Image();
            wheel3.src = "https://codehs.com/uploads/a4b9e60715ec4cb109454ee69e01abda";
            var wheel4 = new Image();
            wheel4.src = "https://codehs.com/uploads/883ff30d7d8a573618ef4494ecab263a";
            var wheel5 = new Image();
            wheel5.src = "https://codehs.com/uploads/22d34c2dca9e3b7e1539f86c51f0a74c";
            var wheel6 = new Image();
            wheel6.src = "https://codehs.com/uploads/73c33efadf5afba1c057b3b2560d64d4";
            var wheel7 = new Image();
            wheel7.src = "https://codehs.com/uploads/4c91204cb815c375033e7c78901c95d1";
            var wheel8 = new Image();
            wheel8.src = "https://codehs.com/uploads/150a147b2dc171204104ae030b4e9e14";
            var wheel9 = new Image();
            wheel9.src = "https://codehs.com/uploads/ac02a9d7f10d5ecfd679aacbf49125c8";
            var wheel10 = new Image();
            wheel10.src = "https://codehs.com/uploads/198777f5d96aab0bf8ad9397ea9e3d0d";
            var wheel11 = new Image();
            wheel11.src = "https://codehs.com/uploads/cebf08e6580b27b142bda25978ab080b";
            var wheel12 = new Image();
            wheel12.src = "https://codehs.com/uploads/4073f3205855e1c4d595a5e690cad64d";
            var wheel13 = new Image();
            wheel13.src = "https://codehs.com/uploads/2cf6947813677c4fa85a6fbbbf44690f";
            var wheel14 = new Image();
            wheel14.src = "https://codehs.com/uploads/fbf030631eaa1ae1b10e43ed5b5bbebb";
            var wheel15 = new Image();  
            wheel15.src = "https://codehs.com/uploads/676d82c576e75065db305a3a265a836e";
            var wheel16 = new Image();  
            wheel16.src = "https://codehs.com/uploads/effe36193deaa8076adbd1f185f2d513";
            var wheel17 = new Image();  
            wheel17.src = "https://codehs.com/uploads/57d5ab7a9fc9867b24602ac8592f0af4";
            var wheel18 = new Image();
            wheel18.src = "https://codehs.com/uploads/4225a82d3ceb00411fdab81c6807fdd6";
            var wheel19 = new Image();  
            wheel19.src = "https://codehs.com/uploads/8ae63df409ba56a3b4c8d196527aefea";
            var wheel20 = new Image();  
            wheel20.src = "https://codehs.com/uploads/8ae63df409ba56a3b4c8d196527aefea";
            var wheel21 = new Image();  
            wheel21.src = "https://codehs.com/uploads/e5bfd3b942c0add1c10b16ab246ba679";
            var wheel22 = new Image();  
            wheel22.src = "https://codehs.com/uploads/946712f15fcf72ef89fd4be3503cb04a";
            var wheel23 = new Image();  
            wheel23.src = "https://codehs.com/uploads/6d122105787152123d5b5fb81dec45df";
            var wheel24 = new Image();  
            wheel24.src = "https://codehs.com/uploads/8f23a8ba1d819c239f22f12636c9d926";

            
            
            
            wheelImages = [wheel1, wheel2, wheel3, wheel4, wheel5, wheel6, wheel7, wheel8, wheel9, wheel10, wheel11, wheel12, wheel13, wheel14, wheel15, wheel16, wheel17, wheel18, wheel19, wheel20, wheel21, wheel22, wheel23, wheel24];
            
            function showImage(wheelNum){
                var canvas = document.getElementById("myCanvas");
                var ctx = canvas.getContext("2d");
                ctx.drawImage(wheelNum, 0, 0, 200, 200);
            }
            function animateWheel(){
                // Spins wheel and picks random number between 0 and 23.
                spinResult = Math.floor(Math.random()*wheelOfFortune.length);   
                      
                setTimeout(function(){showImage(wheelImages[1]);}, 400);
                setTimeout(function(){showImage(wheelImages[2]);}, 800);
                setTimeout(function(){showImage(wheelImages[3]);}, 1200);
                setTimeout(function(){showImage(wheelImages[4]);}, 1600);
                setTimeout(function(){showImage(wheelImages[5]);}, 2000);
                setTimeout(function(){showImage(wheelImages[6]);}, 2400);
                setTimeout(function(){showImage(wheelImages[7]);}, 2800);
                setTimeout(function(){showImage(wheelImages[spinResult]);}, 3200);
            }
          
            // Change variables to next player.
            function nextPlayer(){
                if(playerTurn == 2){
                    playerTurn = 0;
                }else{
                    playerTurn++;
                }
                document.getElementById("whoTurn").innerHTML = "It is now " + players[playerTurn] + "'s turn!";

            }
            
            // This can be used in multiple locations.  It's job is to look at the guesses that have occurred
            // and reveal any letters in the puzzle that match the guesses.
            var guesses = [];
            var puzzleBoard;
            var puzzleMatches;
            function updatePuzzle(){
                var found = false; // keep track if letter is found.
                // Reset board to recreate it.
                puzzleBoard = "";
                puzzleMatches = 0;
                // Loop through the puzzle letter by letter checking all of the guesses to see if it exists.
                // The puzzle needs to exist for this to work. Don't put it before puzzle is picked.
                for(var i = 0; i < puzzle.length; i++){
                    found = false;
                    for(var j = 0; j < guesses.length; j++){
                        if(guesses[j] == puzzle[i]){
                            found = true;
                            puzzleBoard = puzzleBoard + guesses[j];
                            if(guesses[j] == playerGuess){
                                puzzleMatches++;
                            }
                        }
                    }
                    if(found == false){
                        puzzleBoard = puzzleBoard + " _ ";
                    }
                }
                document.getElementById("puzzle").innerHTML = puzzleBoard;
            }
            
            // This is a shortcut attempt to just solve and not guess letters any longer.
            function solvePuzzle(){
                var answer = prompt("What do you think it is?");
                if(answer == puzzle){
                    document.getElementById("announcer").innerHTML = "That is correct! " + players[playerTurn] + " won this round!"; 
                    // reset current round scores to zero and convert winner's score to total.
                    playerTotalScore[playerTurn] = playerCurrentScore[playerTurn];
                    playerCurrentScore[0] = 0;
                    playerCurrentScore[1] = 0;
                    playerCurrentScore[2] = 0;
                    updateScore();
                    document.getElementById("whoTurn").innerHTML = "GAME OVER."    
                }else{
                    document.getElementById("announcer").innerHTML = "Incorrect. You lost your turn.";
                    nextPlayer();
                }
            }
        </script>
    </head>
    <body onload="loadScreen()">
        <h1>Wheel of Fortune</h1>
        <canvas id="myCanvas" width="200" height="200" style="border:1px solid #000000;"></canvas>
        <h3 id="wheel"></h3>
        <b><p id="totalScore"></p></b>
        <hr>
        <p id="roundNum"></p>
        <h1 id="puzzle"></h1>
        <p id="category"></p>
        <hr>
        <b><p id="roundScore"></p></b>
        <h2 id="whoTurn"></h2>
        <p id="announcer">Welcome to the Wheel of Fortune! This is a 3 player game.  Press <b>Start</b> to play!</p>
        <span id ="startButton"><button id="start" type="button" onclick="start()">Start</button></span>
        <button id="spin" type="button" onclick="takeTurn()">Spin Wheel</button>
        <button id="solve" type="button" onclick="solvePuzzle()">Solve Puzzle</button>
        
    </body>
</html>
