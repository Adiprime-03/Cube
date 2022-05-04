Project description

This project is meant to simulate a 3*3 Rubik's cube. The cube, a popular children's toy created in the 70's and popularized by Erno Rubik, has captured the imagination of puzzle enthusiasts and mathematicians everywhere. Our project aims to create a virtual version of the cube and allow users to explore the puzzle. The project also contains an algorithm to solve a scrambled cube and generate a solution. The user may also compete with the computer to solve the cube in the shortest possible time. The cube consists of a 3*3*3 matrix with each element consisting of six faces operations on the matrix are defined in accordance with the legal moves of a cube as defined by the WCA(World Cubing Association). 

The cube has a total of 45 quintillion permutations ignoring rotations. Access is strictly controlled to ensure that the operations performed on the matrix are legal. The moves are represented by the standard notations as proscribed by the WCA. 









Classes Used

Class block-
Class block defines a single block with 6 faces. These faces have colours. So, 27 blocks make a cube. This is important as the computer creates a cube even though it may represent it or not. This shows an important aspect of object oriented programming.


Class cube-
This cube calls an array of class block to create the virtual cube. It also contains many functions to build the cube, update its position, movement functions, functions to check the status of the cube.








Functions Used


void get_faces(): This function gets the faces of the cube as 2 dimensional integer arrays.
int get_pos_of(int id): It locates a given block whose ID is sent as a parameter. It returns the current position of the searched block.
Int get_id_of(int pos): A certain position on the Cube is passed as a parameter. The function then returns the ID of the block at that position.
Int get_col_of(int pos, char f): It takes the position and face of a block as parameter whose colour the function returns.
Int is_correct_pos(int id): The function takes the ID of a particular block. The function then checks if the block is situated in its correct position.
Int is_correct_block(int pos): A position on the cube is passed as a parameter. The function then checks if the block in that position is its correct location on the cube.
Void get_faces(int a[][6][6]): It takes the colours of the faces in the cube and stores it in an array.
Int face_solved(int [3][3]): It checks if a given face is solved.
Int is_solved(Cube&amp;): It takes the reference of a cube as a parameter. It returns 1 if the cube is solved, otherwise it returns 0.
Void paint(): This function initializes the colours on each face of the cube.
Void update(): After each movement this function updates the current position of each block on the cube.
Void build_cube(): This functions assigns each block on the cube a unique ID and paints the faces of the cube.
Int is_face(int, Cube&amp;) : This function takes the ID of a certain block and a reference of the cube as parameters. It checks if the given block is present on the face of the cube.
Int is_down(int, Cube&amp;) : This function takes the ID of a certain block and a reference of the cube as parameters. It checks if the given block is present on the bottom of the cube.
Int is_up(int, Cube&amp;) : This function takes the ID of a certain block and a reference of the cube as parameters. It checks if the given block is present on the top of the cube.
Void turn_to_face(int , Cube&amp;): This function takes the ID of a certain block and a reference of the cube as parameters. It uses the movement functions to turn the cube until the given block is at the face of the cube.
Void r(),f(),b(),l(),u(),d(),ri(),fi(),bi(),li(),ui(),di(),x(),y(),z(),xi(),yi(),zi(): These define the movement of the cube.
Void orient(Cube&amp;): It takes the reference of a cube as the parameter. This function uses the movement functions to orient the cube in such a way that the white centre faces the top and the blue centre is to the face. 
Void white_cross(Cube&amp): It takes the reference of a cube as the parameter. It uses the movement functions to solve the white cross on the cube.
void white_corners(Cube &amp;): It takes the reference of a cube as the parameter. It uses the movement functions to solve the corners on the white face.
void second_layer(Cube &amp;): It takes the reference of a cube as the parameter. It uses the movement functions to solve the second layer of the cube.
void align_yellow_cross(Cube &amp;): It takes the reference of a cube as the parameter. It uses the movement functions to align the yellow cross.
void orient_yellow_corners(Cube &amp;): It takes the reference of a cube as the parameter. It uses the movement functions to orient the yellow corners.
void scramble(Cube &amp;): It takes the reference of a cube as the parameter and scrambles the cube using various movement functions randomly.
void solve(Cube &amp;): This function accepts the reference of a cube as the parameter and uses the above mentioned functions to solve the cube.
Void build_copy(): This function is used in the copy constructor which is used to copy the state of the cube in case the user needs to save the game.
void countdown(): This function displays a 5 second countdown on the screen.
Void race(): This function enables the user to race against the computer while solving the cube. The function also displays the scramble algorithm on the screen.
void instructions(): This function displays the instructions and controls to move the virtual cube during simulation.
Void play_around(): This function enables the user to use a virtual cube.

Void printerror1(), printerror2(), printerror3(): These handle wrong input if and when given by the user.
Functions for printing the cube:
The cube is constructed using 27 blocks, and the display functions just print the side of the block which has a colour.
The idea to print the cube is to pass the value of the colours of each block into a 3-D array, which corresponds to a cube, in a specific order, and then passing 
these values into the following functions to display each side with its respective colour.
Void displeft() - This function displays the left side of the cube by printing 9 quadrilaterals.
Void dispright() - This function displays the right side of the cube by printing 9 quadrilaterals.
Void dispfront() - This function displays the front side of the cube by printing 9 quadrilaterals.
Void disptop() - This function displays the top side of the cube by printing 9 quadrilaterals.
Void dispback() - This function displays the back side of the cube by printing 9 quadrilaterals.
Void dispdown() - This function displays the bottom side of the cube by printing 9 quadrilaterals.






Files Used

Auto_scramble.txt - Used to store and show all the scrambles generated by the computer in that session.

Present_scramble.txt - Used to print the current scramble the user/computer is about to solve.

Instructions.txt - Used to store and print the instructions for using the simulation of the cube.

Pause.dat - Used to save the cube’s position when the user saves it and also used to launch the game from the saved position. 
