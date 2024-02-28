Features:
- A "ActivateLaserRay" variable in the VRPawn class. Activates laser ray functionnality if true
    - Laser ray starts at player's head and points in the same direction as the camera
    - Laser ray destroys all movable object that it comes in contact with
- Robotic arm with a base, arm and forearm component
- BP_movable_object class
    - Grabbable with virtual hands
    - If X button is pressed while one is held
        - Object will turn red
        - BP_movable_object actor with the same static mesh will spawn at a random location in the world
    - If thrown at another BP_movable_object actor, will change static mesh to the one of the hit object

Scene (Level_01):
- A navigable virtual world with a floor, a wall and a few static objects
- 5 instances of BP_movable objects
- 5 static objects behind the wall