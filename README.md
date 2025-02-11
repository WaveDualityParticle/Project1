# Project1

Day 1:

- Migrated Assets
- Made new blueprint for the Target Static Mesh
- Used On Component Hit (Static Mesh) function to print a string. A Cast to Projectile between the print. Which allowed to a string
  to be printed if the projectile hit the target.
- String being "Target Hit" or "Success"
- 
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
Heres how it looks like now...
![image](https://github.com/user-attachments/assets/8bb67876-f12c-48bf-ab18-55d51fe59d4f)


Day 3:

Using Append String function so that the score bar looks like Score: CurrentScore
![image](https://github.com/user-attachments/assets/1e7a4c05-1410-4421-a45d-65b3d20f2802)
It should now look like this:
![image](https://github.com/user-attachments/assets/32c23829-db27-436d-97c0-7cc41bcf6709)
- Now create a new variable called MaxScore this will allow us to make a win screen for the user.
- Create a New Parameter in our UpdateScore custom event and name this MaxScore
  ![image](https://github.com/user-attachments/assets/47b180f9-8ac3-42a6-91e2-17494444846f)
  In the Target GM blueprint add these changes
  ![image](https://github.com/user-attachments/assets/f58e3aa7-2914-41bc-9d01-702a573f701a)
Basic Logic for Win screen checking if the CurrentScore = MaxScore using == operator.
![image](https://github.com/user-attachments/assets/a222494d-2ae6-4494-821f-e991fa043987)
Now lets create a widget for the win screen that would pause everything for the user.
Make a new widget blueprint for the UI.
Here is a simple Win Screen UI

![image](https://github.com/user-attachments/assets/3bb65e12-c4cc-48a5-bbde-754bf2ec5277)

Now go back to Target Game Mode... and then do the same as before for the Score... create a widget then add to 
viewport. Use the promote to variable short cut.

![image](https://github.com/user-attachments/assets/ad1d68d6-6b22-4773-a5cd-f589eac4e816)










