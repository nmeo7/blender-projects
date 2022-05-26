# 3D pipeline

1. prepare the story
2. do some kind of animatrix, maybe previz in my case.
3. design the characters, review the story, the environment, etc.
4. do modeling, rigging, facial riggings, surfacing (texturing).
5. animation - use some references in case needed.
6. extra - crowds, characters fx (everything else that moves that is not the character), explosions, footprints, matte painting, etc.
7. lights => i will preferably shade it 2d
8. image finaling - correct some things - may omit
9. music / sound design. can differentiate pro from amateur.


# Blender tricks

## material:

touch the roughness for some reflection.
then subsurface things.

Light > cast shadow or not.

Fake bumps: Noise node > vector displacement / height > material output displacement
Real bumps: material > settings > displacements and bumps

also for bumps use displacement node and put it in the output displacement, and in the texture/material, change displacement from bump only to displacement and bump.

bumps: displacement node > output displacement
then material  > displacement > displacement and bump


Making glass material in principal shader: change the transmission value. Then play with roughness.
1. roughness - 0, transmission - 1
2. turn on screen space refractions under settings, then screen space reflections in render properties, also refraction inside

you can use the https://github.com/domlysz/BlenderGIS thing for the terrain.

face builder: keentool plugin.

use the bloom thing in eevee
depth of field: have an empty for focus, then camera > depth of field > object > change focus object. then also choose the size.

## texture paint:

image editor > create new image
active tool and workspace settings > brushes settings > texture > mapping > stencil
under texture, add new texture

go to texture paint, create new image, draw on it then save
texture tab, add image, mapping from tiled to stencil.

## must use nodes:

texture coordinate node, colorramp, noise texture, voronoi, mix rgb node, bump node > into normal - texture coordinate node, mapping node, gradient texture, colorramp all the way
texture coordinate node: position textures on 3d objects.

geometry nodes: separate geometry, attribute nodes, transfer attribute node, align euler to vector and normal into the vector, set material, curve to mesh, noise all the way
from the group input you can create custom parameters
m to mute a node, dotted line means it is looping
curves all the way, resample curve then do instance on points after; space by length.
realize instances

new collection with bezier curve, create new geometry.
convert curve to mesh
curve radius - factor


# hard surface modelling:

to the cube; you can add a cast modifier to make it more cubish.
shift + e > creasing a vertex.
bevel: ctrl b, ctrl shift b
use bevel and subsurface modifiers in combinations.
you can also add bevel modifier for edges. limit method > angle
bevel, segments, limit by angle.


inside shader editor > object > world > add a mapping node and a texture coordinate node > then play with it.

alt + D : duplicated objects with same mesh information, where ctrl + D will generate completely new mesh and stuff.



# addons

bsurfaces addon
f2
looptools

n > edit > initialize > draw > add surface


# smoke
create domain object, continuously do free all and bake all, change resolution divisions, turn on noise, turn on disolve to make smoke disappear after some time
create flow object, make it inflow
add material to the domain, use principle volume shader and connect volume into volume
render edits > volumetrics > make tile size very small, also volumetric shadows
change color attribute of the material to temperature

fire vorticity, reaction speed

temperature difference: how fast or how slow the smoke will rise
use texture to emit smoke


hardware that carry light and transmitted into your contiousness in forms of vibrations in your speakers, etc.




# misc

always have a blurry foreground element in your scene
gradient or solid color materials
smear or motion blur

use render farms



# NFTs:

who owns your IG account? what can they do about it? (eg. donald trump, andres iniesta, etc.)?
how much is it worth to you?
but how about we decentralize it? that's the crypto thing.

what is money, if not a symbol? what is the value of likes, if not something we agreed on? how about we now agree on something that is decentralized and traceable?

make artificial scarcity
Don’t be fooled by plug and plays made easy, they are made by billion dollar companies!



# lighting

blender lighting: things change dramatically when there is somethings the light can bounce off of - there is nothing in space, that's why it is dark on the other side of the moon.

change color management look to high contrast, exposure, etc.

soft light / soft shadows: you make the lamp much bigger

blender eevee options: enable ambient occlusion, bloom, screen space reflections
shader for the world



# UX

Tell stories, create emotions: even engineering is storytelling.
Appeal (cognitive easing) makes you feel right at home and generates further interest.

Use basic shapes, quick actions like one click copy and precognitive ux, clear feedback, well defined inputs, emojis and graphics, particles and color, negative space, consistency and contrast, repetition, symmetry, balance, proximity, animation. Keep everything simple, always use a reference and respond to feedback.
Be accessible and inclusive, responsive, use placeholders for the future, recognition over recall, prevent errors rather than fix them. Use breadcrumbs & minimal forms.

Composition: Rule of thirds, leading lines (that converge to the subject), foreground, focal length and aperture, balance (size, contrast, saturation), movement, color grading. The golden ratio all the way.
Post processing: vignette, glow, blur, flare, motion blur
Lighting: 3 point lighting

Use short lines of texts, one paragraph explainer (twitter sized) and images.


# bottom line

=> Learn the rules carefully so that you can break them properly.
Cleanliness is next to godliness. 
