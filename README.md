# ChessBoard
initial commit
# NAME: DOLLY YADAV
# URN : 1805504 , CRN : 1821018
# CHESSBOARD PROBLEM
import numpy as np
array1 = np.ones(64)
array2 = array1.reshape(8,8)
print("#*#*#*#*#*#*#*#*#*#*#*#*#*#")
for i in range(0, 8):
    for j in range(0,8):
        if (i+j) % 2 == 0:
            array2[i][j] = 0
print(array2)
print("#*#*#*#*#*#*#*#*#*#*#*#*#")
print("Where do you want to place the queen?")
row = int(input("Enter the row no. from 0 to 7 where you want to place the queen"))
column = int(input("Enter the column no. from 0 to 7 only"))
print("*#*#*#*# let us begin!! #*#*#*#*")

if row<8 and column < 8:
    array2[row][column] = 9
    print(array2)
    print("WOW,queen{9} has been placed successfully !!")
else:
    print("OOPS! something went wrong")
    print("PLEASE ENTER VALID NUMBER")
