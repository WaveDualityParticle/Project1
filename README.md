# Project1

Day 1:

- Migrated Assets
- Made new blueprint for the Target Static Mesh
- Used On Component Hit (Static Mesh) function to print a string. A Cast to Projectile between the print. Which allowed to a string
  to be printed if the projectile hit the target.
- String being "Target Hit" or "Success"
  ![image](https://github.com/user-attachments/assets/3dd756e6-8214-416f-ae98-125d2d33d0e6)
- HUD class for crosshair FirstPersonHUD
- Creation of a GameMode blueprint - usage of variables. Variable made is CurrentScore.

Day 2:

- Continuation of the CurrentScore and using the ++ function to increment. (A custom event was made called "AddScore") Which made it
easier to be called.
![image](https://github.com/user-attachments/assets/88a9c608-781d-4c4b-83bf-8a161c4fa234)
- Problem was encountered which was that the player could just hit one target more than one time, therefore a restriction
was needed in order to ONLY call the AddScore Event if that target has not been hit before.
- Therefore a new BOOLEAN variable was required this was called IsTargetHit? only if this condition was FALSE
will the event "AddScore" be called. (Branching (if condition) were used)
![image](https://github.com/user-attachments/assets/531450ba-e21e-4f82-87f8-9eb302b4c7df)
- UI interface to display the score was also required. Here a new widget blueprint for the UI was created.
Here I learnt about anchoring and its use.
![image](https://github.com/user-attachments/assets/e535913b-1649-43d9-97fd-f3c53a412539)
![image](https://github.com/user-attachments/assets/41e600a5-53a1-426d-9fa6-5f8c8e3bf9fb)
Another custom event named UpdateScore was also made.



