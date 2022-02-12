# Bomberman_Game
By Ramesh Tamilselvan

Constraints: Use Capital letters for positions and integer for count values

This program that I had written can pass all the test cases given in the question upto Level 5

Completed Upto 5 Levels given in the question

Steps to run the program

Step 1: Enter the inputs
  mSize = 12;
  player = "CB";
  key = "FD";
  vCount = 3;
  villain[0]="BI";
  villain[1]="DF";
  villain[2]="BE";
  bCount = 6;  
  brick[0]="DD";
  brick[1]="ED";
  brick[2]="FB";
  brick[3]="FF";
  brick[4]="GB";
  brick[5]="HD";
  rCount = 2; //Bomb Range + 1 Power
  range[0]="BD"; //Power 1 Location
  range[1]="EB"; //Power 1 Location
  dCount = 2;  //Diagonal Power
  diag[0]="CD"; //Power 2 Location
  diag[1]="CF"; //Power 2 Location
  bombCount = 2; //Bomb Count + 1 Power
  bombs[0]="DC"; //Power 3 Location
  bombs[1]="DE"; //Power 3 Location
  dyCount = 2; //Dynamite Count
  dynamo[0]="FC"; //Dynamite Location
  dynamo[1]="GD"; //Dynamite Location

Step 2: After getting required position of variables now you can move
  W - Move up
  S - Move down
  A - Move left
  D - Move right
  Q - Move diagonally up left
  Z - Move diagonally down left
  E - Move diagonally up right
  C - Move diagonally down right
  X - Ordinary Bomb
      1-Plant
      2-Detonate
  T - Time Bomb
      Int value - After the number of steps that you moved the bomb automaically blast 

Test Cases:

Level 1:

T1: To check whether the map prints correctly
mSize = 12;   //Map Size
player = "CB";    //Player Location
key = "FD";    //Key Location
vCount = 3;   // Villain Count
villain[0]="BI";   //Villain Location
villain[1]="DF";  //Villain Location
villain[2]="BE";  //Villain Location
bCount = 6;   //Bricks Count
brick[0]="DD";  //Bricks Location
brick[1]="ED";  //Bricks Location
brick[2]="FB";  //Bricks Location
brick[3]="FF";  //Bricks Location
brick[4]="GB";  //Bricks Location
brick[5]="HD";  //Bricks Location

T2: To check whether any element on top of other element
mSize = 12;
player = "CB";
key = "CB";
vCount = 3;
villain[0]="BI";
villain[1]="DF";
villain[2]="BE";
bCount = 6;
brick[0]="DD";
brick[1]="ED";
brick[2]="FB";
brick[3]="FF";

T3: To check whether any element on top of other element

mSize = 12;
player = "CB";
key = "FD";
vCount = 3;
villain[0]="BI";
villain[1]="DF";
villain[2]="BE";
bCount = 6;
brick[0]="DD";
brick[1]="ED";
brick[2]="FB";
brick[3]="FB";

T4: To check whether any element on top of other element

mSize = 12;
player = "AC";
key = "FD";
vCount = 3;
villain[0]="BI";
villain[1]="ED";
villain[2]="BE";
bCount = 6;
brick[0]="DD";
brick[1]="ED";
brick[2]="FB";
brick[3]="FF";


Level 2:

Input:
mSize = 12;
player = "CB";
key = "FD";
vCount = 3;
villain[0]="BI";
villain[1]="DF";
villain[2]="BE";
bCount = 6;  
brick[0]="DD";
brick[1]="ED";
brick[2]="FB";
brick[3]="FF";
brick[4]="GB";
brick[5]="HD";

T1:
Move to EB. And Plant a bomb check whether brick alone destroys

T2:
Move to DE. And Plant a bomb check whether side brick and villain alone destroys

T3:
Move to FE. And Plant a bomb check whether right brick alone destroys

T4:
Plant a bomb near the player and detonate it. Check whether Player dies.

T5:
Check whether the player able to plant only one bomb


Level 3:

Input:
mSize = 12;
player = "CB";
key = "FD";
vCount = 3;
villain[0]="BI";
villain[1]="DF";
villain[2]="BE";
bCount = 6;
brick[0]="DD";
brick[1]="ED";
brick[2]="FB";
brick[3]="FF";
brick[4]="GB";
brick[5]="HD";
rCount = 2; //Bomb Range + 1 Power
range[0]="BD"; //Power 1 Location
range[1]="EB"; //Power 1 Location
dCount = 2;  //Diagonal Power
diag[0]="CD"; //Power 2 Location
diag[1]="CF"; //Power 2 Location
bombCount = 2; //Bomb Count + 1 Power
bombs[0]="DC"; //Power 3 Location
bombs[1]="DE"; //Power 3 Location

T1:
Move to EB get Power 1 and plant a bomb at EB and move to BB.  Detonate the bomb
and Check whether the bomb has blast range 2 which destroys the bomb at FB and GB

T2:
Move to EB get Power 1, Move to BD get Power1, Move to CD get Power 2 and Move to
DE get Power 3. Then plant bomb at DE itself and Move to DB. Detonate the Bomb.
-> Destroyed  places DD,ED,DF,GB
Note: Make sure you didn't get power 3 at location DC

T3:
-> Move to EB get Power 1, Move to DC get Power 3, Move to CD get Power 2, Move to
BD get Power1, Move to DE get Power 3. Place a bomb one at DE and another at EB.
Then move to BB to detonate the bombs.
-> Destroyed  places DD,ED,DF,GB,FB,BE


Level 4:

Input:
mSize = 12;
player = "CB";
key = "FD";
vCount = 3;
villain[0]="BI";
villain[1]="DF";
villain[2]="BE";
bCount = 6;
brick[0]="DD";
brick[1]="ED";
brick[2]="FB";
brick[3]="FF";
brick[4]="GB";
brick[5]="HD";
rCount = 2;
range[0]="BD";
range[1]="EB";
dCount = 2;  
diag[0]="CD";
diag[1]="CF";
bombCount = 2;
bombs[0]="DC";
bombs[1]="DE";
dyCount = 2; //Dynamite Count
dynamo[0]="FC"; //Dynamite Location
dynamo[1]="GD"; //Dynamite Location

T1:
-> Move to BD get power 1, Move to CD get power 2, Move to DE get power  3. And place
bomb in DE itself. Then Move to BB
-> Destroyed  places DD,ED,DF,GB,FB,FC,GD,HD


Level 5:

Input:
mSize = 12;
player = "CB";
key = "FD";
vCount = 3;
villain[0]="BI";
villain[1]="DF";
villain[2]="BE";
bCount = 6;
brick[0]="DD";
brick[1]="ED";
brick[2]="FB";
brick[3]="FF";
brick[4]="GB";
brick[5]="HD";
rCount = 2;
range[0]="BD";
range[1]="EB";
dCount = 2;  
diag[0]="CD";
diag[1]="CF";
bombCount = 2;
bombs[0]="DC";
bombs[1]="DE";
dyCount = 2;
dynamo[0]="FC";
dynamo[1]="GD";

T1:

-> Move to EB get Power 1, Move to DC get Power 3, Move to CD get Power 2, Move to
BD get Power1, Move to DE get Power 3. Place a timer bomb  at DE . Then move to BC
to detonate the bomb (Which automatically blast).
-> Destroyed  places DD,DF

