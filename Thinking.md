## What

So let's imagine some sandbox where we could move thing around. Like conveyour belts in factorio. What would be important to make it fill endless in depth and opportunities? Yet would not create paralysis from difficulty of learning it? We can approach this question from different starting points.

## How to approach

First one - let's imagine some cool scenario where moving stuff is important? 

Like if it is some kind of futuristic facility where stuff is produced and moved around? it can be details of robots that march into the battle? Like automatic factory of machines that create its helper bots to scavenge battle field and transform raw materials into deadly weapons?

Like if it is some kind of inter-world crossportal system for aliens of all sorts? and you have to deliver them from on portal to another without them being stuck for too long?

Or in a simpler way? What if a question is about moving cars on a road? And they have to visit places, transport something and then leave to some other place beyond map?

Second one - let's design system or visual language to describe components that could be assembled by some rules to build any logistical system that we want. It would force to choose concepts, rules, limitations, and interactions.

G > > > > T > > > > C
v
v
v
> > > > >

Third one - fuck it let's code something up. Make something that works and try to add things up.

## How I go

I am not that kind of guy to start with some fictional description, yet I am not saying it is wrong or has some disadvantages over any other. To each their own or something like this. I do think that coding without plan is hard for me so I would choose second and third approach and would switch between them when I want.

## First steps

So there are at least two types of things in this sandbox:
 * things that ARE moved by logistical system
 * things that MOVE things around

Each thing that moves something has to have a limit of how many things it can hold at single moment in time. And for simplicity sake I decided that ONLY ONE item can be held by basic moving-things.

So interesting question. Should it be square grid or hex grid? The only possible problem I see is that circle in hex mode is easier to draw. And drawing things in squared grid is almost like typing and can be  prototyped even in text file... but is it better?

Also coordinates system is a bit off with hex-grid? if previously it was like x and y. Is cartesian system still good enough for hex? holly molly geometry is superfucked without cartesian system and there are versions of madness:
 * https://math.stackexchange.com/questions/2254655/hexagon-grid-coordinate-system
 * https://homepages.inf.ed.ac.uk/rbf/CVonline/LOCAL_COPIES/AV0405/MARTIN/Hex.pdf
 * https://www.redblobgames.com/grids/hexagons/

Yet it feels that it can give some issues with rendering of rectangles it can give some new sense of visual style for arranging visual elements on hex based grid.

I also thought about angled isometric rendering which gives sort of different look on things but it is still square-base grid and I just want to try something else for now.

## Hex-grid with coordinates?

Indeed it is a problem how to give unique coordinates to hex grid and not try to shove cartesian system where it does not help.

One funky idea that I like right now is to look at these hexes as sort of pyramid of cubes and each hex is a cube with its x,y,z coordinates.

So instead of trying to use x,y we can try to use q,s,r and keep in mind that they correspond to x,y,z of our imaginary cubes in 3d-space.

Easier said than done so I need to prototype something with this idea.