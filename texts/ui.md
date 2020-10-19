# Mass-data editor

Typical features of editors:
* four- or five-part area layout (left, top and right panel, sometimes even bottom + active viewer in the middle) - examples: photoshop, inkscape, gimp, paraview, qgis, blender
* when the setup gets a little more complex, there is visual programming interface (blender - nodes, unreal - blueprints)
* editor handles certian classes of data (bitmap: the actual raster, layers, filters...; 3d: meshes, modifiers, armatures, volumes...)

Would it be possible to build a database encapsulating all city data?

Hypothesis: *We have too much data, too many classes, and too many parameters which prevents us from creating a complete system for all city data. There will always be a meaningful combination of data classes which won't be supported by the city system.* 


Questions:
* are there any editors for big-data processing? - the data is typically handled using any database model + language for data manipulation - which is not really user-friendly unless you know what you're doing - why is that? because given a blank canvas, the user never knows how to start unless he knows the tools, even if he knows his goals 
* is it possible to reverse the pipeline and guide a user who knows their goal but doesn't know how to achieve it? - the problem is there is a billion meaningful  objectives, programming a custom solution for each objective individualy would take ethernity
* can we somehow design an interaction model that would guide the user through the creation process, even though the system itself doesn't have a pipeline for every possible objective?
