# Ex.No: 5 Create a player Movement Script in unity 
### DATE:                                                                            
### REGISTER NUMBER :212222040047
### AIM: 
To write a program to create a player movement in unity.
### Algorithm:
1. Create a New Unity Project by Open the  Unity Hub and create a new 3D Project,Name the project (e.g., PlayerMovement).
2. Create the Moving Object
   In the Hierarchy, right-click → 3D Object → Capsule (or Sphere).
   Rename it to Player 
4. Adding the Player Movement Behavior Script
   Create the Script-In the Project Window, go to the Assets folder.
   Right-click → Create → C# Script.
5. Write a script for player behavior and save it
6. Attach the Script
   Select player in the Hierarchy - Drag & Drop the playerBehavior script onto the Inspector Panel.
7. Run the game 
8. Stop the program
    
### Program:
```
using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class Player_movement : MonoBehaviour
{
    // Start is called before the first frame update
    public float speed;
    void Start()
    {
    }

    // Update is called once per frame
    void Update()
    {
       float xdir = Input.GetAxis("Horizontal") * speed;
      float zdir = Input.GetAxis("Vertical") * speed;
      transform.position+=new Vector3(xdir, zdir); 
    }
}

```
### Output:

![image](https://github.com/user-attachments/assets/c6a845ff-602d-46c3-90cb-e46feebf5494)

![image](https://github.com/user-attachments/assets/1ea9886a-e746-48b5-a156-b59db761666f)

![image](https://github.com/user-attachments/assets/b4d7e0d9-530a-4600-a9fe-05ca0fb4cd3a)

![image](https://github.com/user-attachments/assets/1ca006cb-1478-464e-8df7-5d20febd87d7)


### Result:
Thus the simple movement behavior was implemented successfully.
