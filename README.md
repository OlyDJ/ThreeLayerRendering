## Three Layer Rendering - Blender Add-on

Fast and low-resources interface to manage View Layers render settings. No need to switch between View Layers, and all related settings unified.

Automatically create Composition Node with all passes mixed, saving you a lot of tedious time.

Automatically splits geometry into three different view layers (Background, Foreground and Focus), giving the ability to do professional renderings in just a few seconds by pressing 2 buttons. It works by measuring distance between the camera and the selected focus object, so it doesn't matter if the focus object has animation. And it works with timeline camera markers.

TLR splits meshes, surfaces, meta-balls and texts. For objects with Geometry Nodes, there is Smart Geo Nodes option, which will try to find the "first" Instances On Points node, and connect a group to its Selection input socket. I've not found a way to know which Instance On Points node is the correct if it is not in the root of GN modifier, so if that node is anywhere else (a group inside the node tree) this method will not work. It is better for performance to not create some instances, instead of deleting them later.

### Features

Support for Blender 4 +
- Splits geometry into 3 different layers (Background, Foreground and Focus).
- Creates View Layers for each one automatically.
- Create new View Layer for selected objects or active collection with just one click (recursive collections included).
- Interface to switch between View Layers options directly, without actually change the active View Layer (which is time and resource saving).
- Change View Layer passes directly.
- Change Exclude, Hide In Viewport, Holdout and Only Indirect of any collection directly for selected View Layer.
- Camera Culling.
- Change View Layers order.
- Automatic Composition Node from scene. Create a composition node group, and mix all layers and passes in the given order inside of it. 
- Automatic Composition Node from EXR files. YES!!! Select a MultiLayer EXR file, set correct order for layers and save a lot of time by pressing just one button.


### Why I created TLR?

It had been a long time since I asked myself: How the hell professional studios render the scenes? Of course it's all about layers. The more splitted the objects, the more control you will have. Even knowing how to render different objects in layers with Blender, It was very hard to do it and get a decent composition. What I learned is that to make it work properly, we must render almost each object on the scene in different layers. 

Well, it is not true. We can tweak some stuff, to get something similar to that professional renders, so I decided to create TLR.

Enjoy it!!!


## Documentation

### Guides and Info

- [How to use this add-on](https://github.com/OlyDJ/ThreeLayerRendering/wiki/How-to-use-this-addon)
- [How to install this add-on - v1.3](https://github.com/OlyDJ/ThreeLayerRendering/wiki/How-to-use-this-add%E2%80%90on-v1.3)
- [How to install this add-on (Outdated)](https://github.com/OlyDJ/ThreeLayerRendering/wiki/How-to-install-this-addon)

### Changelog

- [Changelog](https://github.com/OlyDJ/ThreeLayerRendering/wiki/Changelog)

### Troubleshooting

- [Most asked question](https://github.com/OlyDJ/ThreeLayerRendering/wiki/Most-asked-questions)



