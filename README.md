# Learning-Journal
notes/progress of uni work

## 15-10-2024

made jounrnal on GitHub. coole:3

note to self- follow "tutorial tips" in week 2 (because i will forget)

### making object move in 3D enviroment
((chalk this up properly another time))
create an object
create a C# script called "PlayerMove" when creating it (make sure the class name + script name is the same!)
click on the object and drag your C# script onto the object you want to control.
placing "transform.Translate(Vector3.right);" in void update makes the object travel elsewhere every frame.
adding "float input=Input.GetAxis("Horizontal");" makes the object wait for an input before it starts moving
"transform.Translate(Vector3.right * input);" allows for left and right input.
"transform.Translate(Vector3.right * input * Time.deltaTime" ties the object speed to unity framerate
place "public float Speed = 10f;" in public class to set the object speed
"transform.Translate(Vector3.right * input * Time.deltaTime * Speed);" allows delta time to not be tied directly to unity's framerate
and also allows to control the object.


## 22-10-2024

making progress on tutorials. making a cube interact with a flat surface and moving on it. (tutorial 1)

## 22-10-2024

finishing movment tutorial and workign on pickups tutorial. (tutorial 2)

### making object move and jump on 3D plane
((to be cleaqned up at a later date))
-create one cube and one plane from here:
![image](https://github.com/user-attachments/assets/00444054-2733-4e00-a021-729ce1a80993)

create a C# script and name it "movment". or you can name it something that makes it easy to reference in the future.
![image](https://github.com/user-attachments/assets/6ba912b7-fa98-4a9d-ab39-e14eb3862610)

click on the cube to highlight it and then at the bottom right of the screen click "add component".
go to physics then click on rigid body which will allow the cube to be affected by gravity.

before opening the the movment script, make sure that the cube has the C# script attached to it by checking the inspector while having the cube selected.
it should be at the bottom under "Rigidbody" or above it. if not, have the cube selected and drag it onto the cube to attach it.

just to make sure that things are going as expacted, press the play button at the top of the screen to test if the cube falls onto the plane. if not you may have to go back and check that te cube has a rigid body.

![image](https://github.com/user-attachments/assets/57fe7fb5-9966-4082-bd6f-b42b3436a5ea)

float input = UnityEngine.Input.GetAxis("Horizontal");
transform.Translate(input * speed * Time.deltaTime * Vector3.right);

float input1 = UnityEngine.Input.GetAxis("Vertical");
transform.Translate(input1 * speed * Time.deltaTime * Vector3.forward);

back and forwards movment from code above. forward defines (0, 0, 1) movment. right defines (0, 1, 0) movment.

have these ticked to stop cube rotating on it's own
![image](https://github.com/user-attachments/assets/d6639ea7-c1b7-4a5b-a4a3-bc139742601b)

## 12-11-2024

### working on player health systems

## 3/12/2024

### working on camera tracking tutorial write up

i forgot to note down my progress for the past 2 weeks...
