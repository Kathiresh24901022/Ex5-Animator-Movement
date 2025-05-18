# Ex5-Animator-Movement

## Aim:

To develop a animator movement for a player using unity.

## Algorithm:

## Step 1:
Import necessary models.

## Step 2:
Right-click -> Create -> Animator Controller.

## Step 3:
Open Animator window, define states (Idle, Run, Jump, etc.).

## Step 4:
Use keyframes or Unity's Animation tools to animate transitions between states.

## Step 5:
Drag Animator Controller to the GameObject in the Inspector.

## Program:

Developed By  : SELVAGANESH R

Register No   : 212223230200

## PlayerController:

```
using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class PlayerController : MonoBehaviour
{
    public Animator animator;
    public float InputX;
    public float InputY;
    // Start is called before the first frame update
    void Start()
    {
        animator = this.gameObject.GetComponent < Animator>();
    }

    // Update is called once per frame
    void Update()
    {
        InputY = Input.GetAxis("Vertical");
        InputX = Input.GetAxis("Horizontal");
        animator.SetFloat("InputY", InputY);
        animator.SetFloat("InputX", InputX);
    }
}
```

## Output:

![image](https://github.com/user-attachments/assets/67bc444b-5cf5-4884-8bd8-0c9c3fa3653d)

![image](https://github.com/user-attachments/assets/20d7efe1-f3ab-4901-a21d-5f56864b29a3)

![image](https://github.com/user-attachments/assets/46441085-40b7-4407-b7fa-2ca8dfb90972)

## Result:

An animator movement for a player using unity is developed successfully.
