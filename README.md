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
