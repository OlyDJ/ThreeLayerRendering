Three Layer Rendering - Blender Add-on

Automatically splits geometry into three different view layers (Background, Foreground and Focus), giving the ability to do profesional renderings in just a few seconds by pressing 2 buttons. It works by measuring distance between the camera and the selected focus object.

Press a button to split objects or collections, and press another button to create the View Layers. Once you have all your objects and collections processed, you will find an interface to setup each view layer with its passes and the collections directly, without the need to switch between them (which is a waste of time sometimes).

For objects with Geometry Nodes, TLR will try to find the "first" Instances On Points node, and connect a group to its Selection input socket. I've not found a way to know which Instance On Points node is the correct if it is not in the root of GN modifier, so if that node is anywhere else (a group inside the node tree) this method will not work. I tried this because it is better for performance to not create some instances, instead of deleting them later on. 

Support for Blender 4 +

- Splits geometry into 3 different layers (Background, Foreground and Focus).
- Creates automatically View Layers for each one. 
- Select a camera, or active camera (with timeline markers) will be used instead.
- Option to change Foreground width.
- Option to change Focus object location, rotation and scale.
- Option to change Masks Z location (which depending on the total height of your scene can be usefull). 
- Create a new View Layer for selected objects or active collection with just one click.
- Interface to switch between View Layers options without actually change the active View Layer (which is a time saving depending on the project).
- Option to exclude View Layers directly.
- Change View Layer passes directly.
- Change Exclude, Hide In Viewport, Holdout and Only Indirect of any collection directly.
- Option to show only TLR View Layers.
- Option to show only TLR collections.

Why I created TLR?

It had been a long time since I asked myself: How the hell professional studios render the scenes? Of course it's all about layers. The more splitted the objects, the more control you will have. Even knowing how to render different objects in layers with Blender, It was very hard to do it and get a decent composition later. What I learned is that to make it work properly, we must render almost each object on the scene in different layers. 

Well, it is not true. We can tweak some stuff, to get something similar to that professional renders, so I decided to create TLR.

How to use it?

Select Focus object, select camera (or active camera will be used instead.
Select the objects you want to split (or a collection), and press Process button.
Once you end up splitting, press Create View Layers button.
Now you can render.
All View Layers related settings for the final render will be available without actually switching between them. 
Thats all!

How to install this addon:

- Download the zip file.
- Open Blender and go to Edit - Preferences
- Go to Add-ons Tab.
- Press Install button, and search for the downloaded zip file.
- Select it and press Install
- Just click the box to enable it and you are ready to go.

Enjoy it!!!


