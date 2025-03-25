Scry is, obviously, built on a large stack of internal and external tech. We'll catalogue all the stuff we've made in and around the Unity project, as well as some helpful pieces of information about the systems we use from other sources, like literature from Unity we've found particularly useful.

# Scripts

## Homemade


## Borrowed

### Unity Packages

### AR Foundation Template

# Prefabs

"Prefabricated Game Objects" or something like that. Prefabs are Unity's solution for putting together in-engine lego pieces so you don't have to rebuild GameObjects from scratch.

We have a few different categories for Prefabs in the project.
## Setup

Many scripts attached to certain GameObjects require specific settings before they work the way we'd like them to. By making a prefab, we can save these settings to an asset that we later simply drag and drop into a new Scene and it should work out of the box with no tinkering.

### AR Setup

Unity's XR and AR features have a lot of moving parts, so saving a prefab with our base functionality can help us with a lot of things.
#### [AR Scene Objects](Tech/Prefabs/AR-Scene-Objects)

This prefab saves our GameObjects that hold AR functionality into one object that can be dragged & dropped to initiate the AR & XR functionality we need to play a level using AR.
## Content

Content Prefabs are the Prefabs that let us build interactable objects for experiences. These include our dioramas of 3D models and the attached objects that add features and functionality to them.
### Base Model
The Base Model is where we place imported 3D models. Here we can attach event listeners to them, set up rendering responses like highlights, and organize the model's different mesh components into categorical lists.
### Base AR Prefab
The Base AR Prefab holds a Base Model, and attaches all the things that make it interactable.
## UI

Pre-building UI objects saves a ton of time setting up game events, styling, layout (especially this), and UI response to events.

It's useful to have prefab button, window, text, and other UI element types that match our UI style out of the box and don't need to be meticulously edited before they look right. Plus, UI is great for triggering functionality (as it typically does), so adding hooks for events out of the box is great.

### Layout Elements

### Buttons

### Text