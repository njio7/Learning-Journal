# Learning-Journal
notes/progress of uni work

## 15-10-2024

made jounrnal on GitHub. coole:3

note to self- follow "tutorial tips" in week 2 (because i will forget)

### making object move in 3D enviroment
((chalk this up properly another time))
-create an object
-create a C# script called "PlayerMove" when creating it (make sure the class name + script name is the same!)
-click on the object and drag your C# script onto the object you want to control.
-placing "transform.Translate(Vector3.right);" in void update makes the object travel elsewhere every frame.
-adding "float input=Input.GetAxis("Horizontal");" makes the object wait for an input before it starts moving
-"transform.Translate(Vector3.right * input);" allows for left and right input.
-"transform.Translate(Vector3.right * input * Time.deltaTime" ties the object speed to unity framerate
-place "public float Speed = 10f;" in public class to set the object speed
-"transform.Translate(Vector3.right * input * Time.deltaTime * Speed);" allows delta time to not be tied directly to unity's framerate
and also allows to control the object.


## 15-10-2024

making progress on tutorials. making a cube interact with a flat surface and moving on it. 

### making object move and jump on 3D plane
((to be cleaqned up at a later date))
-create one cube and one plane from here:
![image](https://github.com/user-attachments/assets/00444054-2733-4e00-a021-729ce1a80993)

