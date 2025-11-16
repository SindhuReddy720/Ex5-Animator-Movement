# Ex5-Animator-Movement

## Aim:
To develop a animator movement for a player using unity.

## Algorithm:

## STEP 1:
Import necessary models.

## STEP 2:
Right-click -> Create -> Animator Controller.

## STEP 3:
Open Animator window, define states (Idle, Run, Jump, etc.).

## STEP 4:
Use keyframes or Unity's Animation tools to animate transitions between states.

## STEP 5:
Drag Animator Controller to the GameObject in the Inspector.

## Program:

### Developed by : Pelleti Sindhu Sri
### Register no : 212224240113

## Movement.cs:
```csharp
using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class Movement : MonoBehaviour
{
    public Animator animator;
    public float InputX;
    public float InputY;
    // Start is called once before the first execution of Update after the MonoBehaviour is created
    void Start()
    {
        animator = this.gameObject.GetComponent<Animator>();        
    }

    // Update is called once per frame
    void Update()
    {
        InputX = Input.GetAxis("Horizontal");
        InputY = Input.GetAxis("Vertical");
        animator.SetFloat("InputX", InputX);
        animator.SetFloat("InputY", InputY);

        
    }
}
```

## Output:

![alt text](<Screenshot 2025-11-16 161020.png>)

## Result:
An animator movement for a player using unity is developed successfully.
