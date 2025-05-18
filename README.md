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
```python
Developed By  : SANJAY M
Register No   : 212223230187
```

## PlayerController:
```python
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
![image](https://github.com/user-attachments/assets/e75ef91d-a9d2-4680-b794-3b2021b71d7d)
![image](https://github.com/user-attachments/assets/5b03c677-f457-4d63-8329-4314e0ef2972)
![image](https://github.com/user-attachments/assets/4ff0e480-db41-449c-ba4b-f4dad308f753)




## Result:

An animator movement for a player using unity is developed successfully.
