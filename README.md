# Search-The-Picture
* The photo taken by the camera is given as a String[], where the x-th character of the y-th
element is the color of the 2 x 2 square whose upper-left corner is at (2*x, 2*y). Colors are
either uppercase letters (’A’-’Z’) or digits (’0’-’9’). Uppercase letters represent terrain features
(floor, chairs, spectators, etc.) and each digit X represents the color of the uniform used by the
X-th team.
* Two squares A and B belong to the same object if and only if there exists a chain of squares
where the first square is A, the last square is B, each pair of consecutive squares in the chain
shares a common edge and all the squares in the chain have the same color. The position of
an object C is the center of its bounding box, where its bounding box is defined as smallest
axis-aligned box that contains all the object’s squares. An object’s area is defined as the sum
of the areas of all the squares that compose the object. An object is a player from the i-th
team if and only if it is colored with the digit i and its area is at least threshold.
* Return a java.awt.Point[] containing all the players in the photo from the k-th team. Each
element should represent a single player and be formatted java.awt.Point(X,Y), where (X,
Y) is the center of the player’s bounding box, and X and Y have no extra leading zeros.
Sort the players in increasing order by x-coordinate. Sort players with the same x-coordinate
in increasing order by y-coordinate.
