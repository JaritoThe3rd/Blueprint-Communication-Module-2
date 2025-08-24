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


<img width="585" height="288" alt="image" src="https://github.com/user-attachments/assets/4e0d8d3c-e4dd-4a90-9b3b-9dabdaba9364" />


But you need to make sure to make an array for your object types.

<img width="1348" height="580" alt="image" src="https://github.com/user-attachments/assets/5012a9e6-a9ff-49f4-b66b-7e3f3706a95c" />

The blue cube has an object type of PhysicsBody, which will not respond from your Line Trace for Object array.

<img width="1695" height="688" alt="image" src="https://github.com/user-attachments/assets/551f6737-e8e3-4eb0-a495-89c8e289dca3" />

But the stair case will have an World Static object type setting, So it will respond from your Line Trace for Object array.

<img width="1549" height="714" alt="image" src="https://github.com/user-attachments/assets/b8fb7607-2e3d-4cac-813f-57d4ba1099ec" />

In the Project Settings > Engine > Collision we can add a custom Object trace.

<img width="1894" height="954" alt="image" src="https://github.com/user-attachments/assets/3611f66e-ad8f-4a96-a7ac-c4a2305e2cd5" />

You might want to click off on the Editor world before the custom trace shows off.


<img width="1301" height="726" alt="image" src="https://github.com/user-attachments/assets/fdf5376b-88cc-41cf-92b0-e91f6940db7e" />

!!! Compile the Blueprint TraceCannon for it to show your custom trace object.


<img width="669" height="126" alt="image" src="https://github.com/user-attachments/assets/19ea679b-9e89-44f7-bbf1-8c55653d9535" />

Beware of complex collision setting from Line trace.

<img width="332" height="43" alt="image" src="https://github.com/user-attachments/assets/ecff9d97-146a-4930-96d1-0565ccde61af" />

Ignores Actors from receiving the trace. It's an array too so you can have multiple ignore actors.

<img width="426" height="458" alt="image" src="https://github.com/user-attachments/assets/7052e348-6b1e-4f0b-9bd1-50d6884250c4" />

More settings for trace objects.


<img width="1073" height="559" alt="image" src="https://github.com/user-attachments/assets/93d1fdb7-14fd-4872-89d0-5b6dedc5dd98" />

<img width="678" height="540" alt="image" src="https://github.com/user-attachments/assets/57448d17-7a7b-4ff2-8200-93a40fc64c7b" />

Multi line trace basically returns multiple hits.

<img width="1908" height="951" alt="image" src="https://github.com/user-attachments/assets/c454867e-035a-43db-9dc5-8e3523f87ad6" />

This is a single line trace channel where it passes through the first white block and then it stops detecting the next couple of blocks.

<img width="1908" height="932" alt="image" src="https://github.com/user-attachments/assets/40222084-503d-42a8-af14-18d46c6fd97b" />

For multi line trace channel it passes and detects multiple objects at once.


<img width="1081" height="573" alt="image" src="https://github.com/user-attachments/assets/fad48a9e-7bbf-4299-a91d-e2dc8d4ad588" />


<img width="940" height="722" alt="image" src="https://github.com/user-attachments/assets/4b139e45-4cfd-487f-8c7c-f95e2e749c0a" />

<img width="842" height="854" alt="image" src="https://github.com/user-attachments/assets/5195a1b4-4ad5-4906-96ec-6cb4937589a0" />

For line trace objects "Location" and "Impact Point" are similar compared to multi line trace.


<img width="1048" height="623" alt="image" src="https://github.com/user-attachments/assets/c358da68-0bbd-4e62-b58a-316091b99399" />


Where it gathers all the data as a group.


<img width="831" height="458" alt="image" src="https://github.com/user-attachments/assets/67ffb25e-c5be-4ff2-a74c-d0546fe12b67" />


<img width="3439" height="1354" alt="image" src="https://github.com/user-attachments/assets/ccdf09d1-be6e-4934-af6b-fe7ac584c65d" />


<img width="1899" height="986" alt="image" src="https://github.com/user-attachments/assets/307ef451-3c73-4f90-bc79-b2ce773843f1" />

Make 2 output variables which are "Verb" and "Noun" for the "Look at" function.


<img width="902" height="834" alt="image" src="https://github.com/user-attachments/assets/a3f2fdc5-8675-4436-a0aa-dd1ba86e3fa8" />

In the "Interact With" function make an input > First Person Character > Object Reference.

 
<img width="1891" height="936" alt="image" src="https://github.com/user-attachments/assets/7a6b4d7f-6cd8-4dd8-9260-fecbf9471017" />

Now we can connect that interactable object which is the door.

<img width="2960" height="792" alt="image" src="https://github.com/user-attachments/assets/7aa50fc3-dc7e-4987-8418-a2ea41cd62b8" />

Go to the door blueprint > Class Settings > Implemented Interfaces > Add "BPI Interface".

<img width="742" height="782" alt="image" src="https://github.com/user-attachments/assets/10504bb5-b7c5-4b8a-a73f-a6b640070414" />

Now you'll see interfaces on your new functions. You basically connected the BPI_Interaface with BP_Door.

<img width="2306" height="1134" alt="image" src="https://github.com/user-attachments/assets/b8295e33-b2a4-49e9-bdac-946d2d36c003" />


<img width="2297" height="884" alt="image" src="https://github.com/user-attachments/assets/5ed22e64-0aca-4e4a-b5d4-e4724cb8d2b9" />

Go to LooAt function > Edit the blueprints for "Verb" into "Open" and "Noun" into "Door".

<img width="1876" height="986" alt="image" src="https://github.com/user-attachments/assets/bb137ce7-a56b-466a-8ae1-beab8e33ef69" />

Remember the pattern of your Interaction Trace blueprints.

<img width="1546" height="601" alt="image" src="https://github.com/user-attachments/assets/68f9a151-6188-4fff-b693-af4d54875b6e" />


<img width="821" height="492" alt="image" src="https://github.com/user-attachments/assets/4c7a32d2-1e75-46e9-a379-0e1a28202441" />


<img width="1129" height="251" alt="image" src="https://github.com/user-attachments/assets/cd24b40e-382d-43af-83d6-6c3fa84f6f06" />

IA_Interact is a boolean whether we're interacting or not two states.

<img width="931" height="278" alt="image" src="https://github.com/user-attachments/assets/1bf85b58-6e45-469b-902f-e4a8a21ec243" />

IMC_Defaule this is for mapping keys and which input.

<img width="3439" height="542" alt="image" src="https://github.com/user-attachments/assets/2efcb71a-bcc6-4375-8310-8dd10c220363" />
<img width="422" height="56" alt="image" src="https://github.com/user-attachments/assets/acac193c-5641-43cc-a77a-6f9eff842843" />
There are existing ones already and add IA_Interact then set to "E" key pressing the keyboard then "E" lastly Save it.


<img width="2206" height="1017" alt="image" src="https://github.com/user-attachments/assets/db8ca7bb-2cdc-4632-8854-6f1920fd0508" />

<img width="2521" height="1088" alt="image" src="https://github.com/user-attachments/assets/8cf56223-07fc-447b-b951-5af1a42615e2" />


<img width="1140" height="626" alt="image" src="https://github.com/user-attachments/assets/950ca601-e20b-4fbe-924e-2fa0d93a9243" />


<img width="3432" height="1320" alt="image" src="https://github.com/user-attachments/assets/2ad3c621-b03f-4dd1-8c25-0a4b4d7e230a" />

if you're having this trace problem just set this up to one frame <img width="912" height="749" alt="image" src="https://github.com/user-attachments/assets/3c062ed0-3dc3-4d8d-bc14-622defe8bddb" />


<img width="912" height="749" alt="image" src="https://github.com/user-attachments/assets/ca2c411c-b9f9-4774-8759-915de875b529" />


<img width="403" height="445" alt="image" src="https://github.com/user-attachments/assets/0f5a5c53-3396-4b21-b8de-2aea10a94fba" />

Beware of development only is for the early stages of your development phase, but when shipping the product you musth avoid it.

<img width="1882" height="927" alt="image" src="https://github.com/user-attachments/assets/671d4af4-b67f-424e-a34b-31aff96b4552" />

<img width="3222" height="1298" alt="image" src="https://github.com/user-attachments/assets/3155f314-9416-4d0e-9ead-2fd35619c93b" />
<img width="862" height="506" alt="image" src="https://github.com/user-attachments/assets/b3825fe5-0fe8-47bc-adc9-cc6e87e59123" />
<img width="865" height="890" alt="image" src="https://github.com/user-attachments/assets/ca13cfb1-871a-4b3f-ac8a-5ad83acf924c" />
<img width="884" height="659" alt="image" src="https://github.com/user-attachments/assets/5f17b50e-1ff8-4f9a-90d0-87b0b4b1d135" />
<img width="867" height="415" alt="image" src="https://github.com/user-attachments/assets/052c0d7e-3b6f-4bf7-becc-a24ef4e6f646" />


<img width="3279" height="953" alt="image" src="https://github.com/user-attachments/assets/49424a20-1511-40fe-90fa-6b81e5753b34" />

Fixing the clipping issue by adjusting it from the viewport within the coin blueprint.

<img width="709" height="458" alt="image" src="https://github.com/user-attachments/assets/253f79f4-337d-42c4-8345-fb461d191b03" />

Adding the rotating component for the coin to rotate similar in crash bandicoot.

<img width="1054" height="545" alt="image" src="https://github.com/user-attachments/assets/31a10932-aebf-4b85-83b8-e167ad1b074c" />

Making the coin dissapear like you grabbed it.

<img width="1421" height="802" alt="image" src="https://github.com/user-attachments/assets/1b23c81e-1763-4c3b-acb7-9e1c3aef1a67" />

!!!!Turns out the coin wasn't dissappearing cuz you need to add a box collision and set that box into "OverlapAll" so the coin gets detected by the player through collision.!!!!


<img width="1809" height="935" alt="image" src="https://github.com/user-attachments/assets/b3c00dd3-674c-4caa-87ed-7965c95c7bdb" />


<img width="731" height="918" alt="image" src="https://github.com/user-attachments/assets/608bba6d-53e4-4b70-9680-45447c53e491" />

<img width="740" height="715" alt="image" src="https://github.com/user-attachments/assets/1d18f693-6dff-4ebe-8857-2d3d83a85481" />

<img width="829" height="506" alt="image" src="https://github.com/user-attachments/assets/2fab15ea-f711-4b39-843b-5ec718f613ae" />

Instead of adding input from the details tab you can just drag the pin onto the "AddScore" function.

<img width="3428" height="1209" alt="image" src="https://github.com/user-attachments/assets/e3d1bc1f-4263-4e04-91b2-e54ac40801f1" />


<img width="2133" height="943" alt="image" src="https://github.com/user-attachments/assets/d81eb807-fcaa-4048-9348-c6b72ef80122" />

We can't find the "AddScore" function from the BP_COIN. <img width="130" height="36" alt="image" src="https://github.com/user-attachments/assets/47178359-3bbe-4033-88c0-d80bc3b89bc8" /> so you need to cast from parent into child class.

<img width="1889" height="995" alt="image" src="https://github.com/user-attachments/assets/d6295584-a0ff-4680-8aeb-dbeed75fb620" />


<img width="778" height="509" alt="image" src="https://github.com/user-attachments/assets/05f4bf78-77ab-4581-9d0d-6e4d0d5ca602" />

<img width="779" height="842" alt="image" src="https://github.com/user-attachments/assets/5777eee5-054c-467d-b885-44ff49366cf6" />


<img width="801" height="614" alt="image" src="https://github.com/user-attachments/assets/e626143a-be40-44c9-bccb-94a2626dca52" />


<img width="830" height="557" alt="image" src="https://github.com/user-attachments/assets/224f4434-8fb5-408c-b669-e67103446314" />

<img width="807" height="545" alt="image" src="https://github.com/user-attachments/assets/04bd9d29-4552-47ba-ab0e-052aebb1c300" />
