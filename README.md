# Computer-Programming-Final-Project
Go to our project ([OurGame - The ZombiNTU](https://github.com/PythonFinalProject/OurGame))

![](https://i.imgur.com/UWpPnSS.png)

## My Contribution Part
Use map created by Tiled editor and build camera perspective for 2P/1P player(s)


![](https://i.imgur.com/NuBjZtA)

There are 3 different types of objects in our maps, Stone, Proof and Block.

-Stone:
It acts as an obstacle for Characters moving on x axis, but an accelerating tunnel for Characters moving on y axis. 

-Proof:
Just as literally, this kind of object is bullet-proof and the bullet will disappear after colliding with it.

-Block:
Different from Stone, Characters can't pass it from any direction, but it's destroyable with bullet.

## Example
`Class TiledMap`\
Clear background created using Tiled editor and load with pytmx

`Class Camera`\
Use camera.update(player_list) to track position of players, then showing on the camera.show surface 

`checkobj1obj2Collision`\
Track if there are collision events e.g. EnemyStoneCollision, BulletProofCollision...
If True then trigger bounce back event or remove map object from background
