# Ex.No: 3  Basic movements in Unity 
### DATE: 27-10-26                                                                         
### REGISTER NUMBER : 212225240054
### AIM: 
 To learn the basic movements translation,scaling and rotation of game objects through code.
### Procedure:
1. Setup the Scene
2. Open Unity and create a 3D Scene.
3. Add three objects:Cube → Rename to Object1 (for movement),Sphere → Rename to Object2 (for rotation).Capsule → Rename to Object3 (for scaling).
4. Add the Script,Create a C# Script → Name it TransformOperations.cs.
5. Write the code for translation,scaling and rotation,save and close the script
6. Save the script
7. Select any empty GameObject (or create one: GameObject → Create Empty).
8. Attach the TransformOperations script to it.
9. In the Inspector, assign Object1 → Drag the Cube,Object2 → Drag the Sphere.Object3 → Drag the Capsule.
10. Run the Scene Press Play ▶️ in Unity
11. Stop the program.
### Program 
```
using UnityEngine;

public class Transformation : MonoBehaviour
{
    // Start is called once before the first execution of Update after the MonoBehaviour is created
    public Transform o1, o2, o3;
    void Start()
    {
        
    }

    // Update is called once per frame
    void Update()
    {
        if (Input.GetKeyDown(KeyCode.Space))
        {
            o1.Translate(2f, 0, 0);
        }
        if (Input.GetKeyDown(KeyCode.A))
        {
            o2.Rotate(0, 10f, 0);
        }
        if (Input.GetKeyDown(KeyCode.D)){
            o3.localScale += new Vector3(2f, 2f, 2f);
        }
        if (Input.GetKeyDown(KeyCode.W))
        {
            o1.Translate(-2f, 0, 0);
        }
        if (Input.GetKeyDown(KeyCode.S))
        {
            o3.localScale += new Vector3(-2f, -2f, -2f);
        }

    }
}

```
### Output:

## Translating movement along x-axis using cylinder object

<img width="1535" height="862" alt="image" src="https://github.com/user-attachments/assets/0096f821-d8ec-4935-b567-d66ad6335e40" />
<img width="1535" height="862" alt="image" src="https://github.com/user-attachments/assets/4a1b56fe-ce7b-4c01-aeb0-09ce6433bbf6" />
<img width="1535" height="862" alt="image" src="https://github.com/user-attachments/assets/353b1adc-6e03-435a-b146-d93eaf861250" />


## Rotating movement using cube object

<img width="1535" height="862" alt="image" src="https://github.com/user-attachments/assets/32ad3cfa-3302-414d-af5a-5b1df61b35ba" />
<img width="1532" height="862" alt="image" src="https://github.com/user-attachments/assets/0b08a788-8226-4511-979d-1e7407268332" />
<img width="1535" height="862" alt="image" src="https://github.com/user-attachments/assets/40c2ad8d-e449-45a2-808e-14611a40f612" />
<img width="1535" height="862" alt="image" src="https://github.com/user-attachments/assets/068fedb0-cdb7-49c0-a897-e64b07068f5e" />

## Scaling movement using capsule

<img width="1533" height="862" alt="image" src="https://github.com/user-attachments/assets/b615e6e2-1214-4e97-bb28-fdfc22a50410" />
<img width="1535" height="863" alt="image" src="https://github.com/user-attachments/assets/3399de9d-f1e7-4179-9c23-995eea12c8cc" />
<img width="1535" height="862" alt="image" src="https://github.com/user-attachments/assets/422d2919-b876-4531-9fa6-0c06bf76c53e" />


### Result:
Thus the basic movement is learned through scripting


