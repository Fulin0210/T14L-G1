# T14L-G1
# Part 1

## Video Demo

Please provide the YouTube link to your [Video Demo](https://youtube.com).

## Minimum Requirements

### Completed

List all the features completed.

1. Gameboard class was created.
2. Character classes were created.
3. Testing of the above classes was completed.

### To Do

List all the features not yet done. Remove this section if there is no incomplete requirements.

1. Create functions to generate game objects as per user demand.
2. Create functions to controle game objects as per user demand.
3. Handle user inputs including unexpected inputs.
4. Handle saving and loading function for the game.
5. Finally test the complete product before submitting.

## Additional Features

No additional feature has been implemented.

## Contributions

List down the contribution of each group members.

### Kawsar

1. Create a random number generator function to make it easy along the way to generate random numbers.
2. Define class to generate the gameboard upon given dimensions.
3. Define super class with the common characteristics.
4. Characters have been facilitated with movement ability through the superclass(Character) methods.
5. Characters are given the got hit behaviour via super class method.
6. Alien, Zombie, Rock and Pod classes were created by inheriting the Character super class with inclusion of some crucial extra characteristics.

### Steve Rogers

1. Zombie movement and attack behaviour.
2. *add more*

### Dr. Strange

1. Implement all game objects.
2. *add more*

## Problems Encountered & Solutions

Problem: Returning a 2D array from a function.
Solution: Whenever an array is created in c++, a dedicated memory location according to the array size gets allocated for the array. And as we keep assigning the values to the array, it stores the values to the previously allocated memory location in a row wise manner. To get an array back from a function in c++ we need to get the pointer to the first object location in the memory. Once we have the first object location pointer we can just keep addin 1 to the pointer to get the next object pointer. And once we have the pointer we can jsut dereferance the pointer to access the actual value that is stored in the memory location. 
Now for a 2D array, we will have an array of arrays. So, we will have an array as the first element of the first array. To access all the elements of the 2D array at first we need to have the pointer to the first element of the container array which is an array itself. So to access the first element of the 2D array we need to access the first array pointer and then the pointer to the first elemt of the first array inside the container array. After we have the pointer to the first element of the first array in the container we can just keep adding 1 to access the next element and to change the row we can just add 1 to the first array pointer.
