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
## Developed by: AHALYA S
## Reg no: 212223230006
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


![image](https://github.com/user-attachments/assets/e4663246-cfa2-4d8b-b9eb-292cd607d604)



![image](https://github.com/user-attachments/assets/3802fb66-9c3b-48b2-b168-d1462a6016d4)



![image](https://github.com/user-attachments/assets/b8836eec-26ff-4271-82fb-2af81e02d317)

## Result:

An animator movement for a player using unity is developed successfully.
