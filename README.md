# Blueprint-Communication-Module-2


<img width="1297" height="656" alt="image" src="https://github.com/user-attachments/assets/0fa49303-fa1d-4f2c-9b07-48090ec1dcc5" />


<img width="743" height="372" alt="image" src="https://github.com/user-attachments/assets/9dba13a2-476e-4f33-8798-632374b0e6f7" />

Add a Cone and a Scene component to your viewport


<img width="1569" height="1085" alt="image" src="https://github.com/user-attachments/assets/e0164467-da6e-4207-be74-191a36aab943" />

In your Eventgraph add "Line Trace by Channel" and you'll be focusing on these <img width="262" height="167" alt="image" src="https://github.com/user-attachments/assets/0e5ed240-0858-43e7-a5de-21a13af520ae" />


<img width="1244" height="688" alt="image" src="https://github.com/user-attachments/assets/6640e791-4f9c-4c3e-80e9-96b2f30b8664" />


We're getting the "Scene" component and connect it to "Get World Location", which is the tip of our cone's location. Which is the start position of our cone where the tip is and where the scene component is placed.


<img width="1582" height="1145" alt="image" src="https://github.com/user-attachments/assets/46e1cede-b8f3-4493-bdd5-232ea34de39b" />


<img width="1335" height="667" alt="image" src="https://github.com/user-attachments/assets/a807c513-475c-4f4c-bac1-fc53ac39b07f" />


Adding "Get Forward Vector" and multiply the length (Make sure to turn into Float data type.)


<img width="1577" height="1258" alt="image" src="https://github.com/user-attachments/assets/2ff7594b-9185-427b-bf3c-f201cca233d3" />

<img width="421" height="112" alt="image" src="https://github.com/user-attachments/assets/b35296b0-7f2e-4b90-9d99-4d144af78a87" />

For the trace lines to stay you need to set Draw Debug Type to "Persistent"


<img width="3437" height="1355" alt="image" src="https://github.com/user-attachments/assets/7a714170-51a5-4776-a6fd-dbeb9f8c033f" />

Now it shoots out a trace line from a cone.


<img width="842" height="453" alt="image" src="https://github.com/user-attachments/assets/f445466e-0145-4cdb-af45-0053747727f1" />


<img width="1168" height="811" alt="image" src="https://github.com/user-attachments/assets/3ee316a9-e565-4aa2-8085-68295434a975" />


<img width="3430" height="1357" alt="image" src="https://github.com/user-attachments/assets/ec24eba0-ec0d-4908-890f-7be68ff74e72" />


<img width="1098" height="519" alt="image" src="https://github.com/user-attachments/assets/45bdb6d1-d233-4f25-b00b-cea4755ddb42" />


<img width="1356" height="641" alt="image" src="https://github.com/user-attachments/assets/cba00ee7-5a68-4fe4-8c85-95c6f2d1dea2" />


<img width="3431" height="1355" alt="image" src="https://github.com/user-attachments/assets/f42d0ce4-c5aa-4e92-8793-33f989a738a1" />


<img width="1107" height="488" alt="image" src="https://github.com/user-attachments/assets/9db6e08a-d0d8-4e28-af4e-0aa467573604" />


<img width="3439" height="1346" alt="image" src="https://github.com/user-attachments/assets/6a197c96-bff6-4e27-926c-49b9e3e84550" />


<img width="867" height="482" alt="image" src="https://github.com/user-attachments/assets/67b46a95-ce72-4288-9ebc-df99705983cd" />


<img width="1668" height="906" alt="image" src="https://github.com/user-attachments/assets/7d9f9b3e-1815-41ac-8d1d-f8009ea7b43a" />

You can make your own trace channels from the project settings.


<img width="661" height="413" alt="image" src="https://github.com/user-attachments/assets/1ad62ae4-54f6-4769-84cc-3421839e342a" />


You want every object in the game would not be interactive so choose ignore.


<img width="452" height="469" alt="image" src="https://github.com/user-attachments/assets/26c46d42-d656-4104-95b3-fe44b6381bad" />

COMPILE FIRST then your custom "Interaction" trace channel will show up in the blueprint of cannon.


<img width="871" height="481" alt="image" src="https://github.com/user-attachments/assets/7cc3f49a-deab-49dd-bd3e-b9de30c97eff" />


<img width="1202" height="464" alt="image" src="https://github.com/user-attachments/assets/0a9d8cd9-02f4-4b51-9a1c-838a2ba55e54" />


The main difference between "Line Trace Channels" and "Line Trace for Objects" is basically object type can be an array and it can trigger multiple interactable objects.
