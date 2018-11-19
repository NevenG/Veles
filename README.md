# Veles
A puzzle box using both physical and software interactions to achieve a final win state

# Naming
Veles, the puzzle, has been named after the major Slavic god [Veles](https://en.wikipedia.org/wiki/Veles_(god)). This name was chosen to highlight Veles' aspects of trickery, magic and wealth and their relations to good puzzle design. The three aspects embody the three stages any engaging puzzle must venture through.

First a puzzle must trick the user by presenting a goal or end-state, while the next step of the puzzle should be obvious the obvious method to achieve that state must be subverted otherwise the user is unaware they are solving anything. 

A puzzles "magic" comes from understanding that it is indeed a puzzle and not just a sequence of operations. While any puzzle is a sequence of operations (in the way a square is a rectangle), the differentiation should come in that a non-puzzle sequences either give no relation between the previous and next actions or it offers no actions to the user other than the next possible action at any stage. In contrast a puzzle should seek to link the last and next actions at all stages. Progressing through a puzzle should require the user to examine the puzzle's state through both observation and analytical lenses and discover the mechanism hidden behind the puzzle which they are acting upon. This stresses a mental connection between user and puzzle not often allotted to mundane objects.

Once a puzzle is solved a user should feel enriched for doing so. Each partial solution should be provided with a clear and gratifying response from the puzzle to show the user they have been successful in some way. Additionally, it should be ensured that the response can not be misinterpreted as back tracking. Likewise, the puzzle should preferably not respond in a way which frustrates the user at any point, ie. a seemingly random reversal of progress. While the statement "you need to spend money to make money" may be true, in terms of puzzles "you need to walk backwards to move forwards" should be avoided and when used it should be minimized to self contained puzzle steps, one puzzle step undoing the progress of another makes the user feel robbed and uncomfortable.

These principals will be kept in mind during development of the Veles puzzle and should be obvious upon the final release how they have been employed. While I hope to make Veles an interesting experience all it's own, it should also function as a learning experience (both for myself as a developer as I seek to understand better puzzles) and for the users of Veles' as the open source nature should allow them to both solve the puzzle blind and to then go back and examine the puzzle in all it's aspects. 

# The Concept

Veles is an attempt to merge puzzle video games with physical puzzle boxes and contains two distinct components. The first of which is the physical box itself. Veles as both an object and a video game will be interacted with using the puzzle box. The box will house a micro-controller, several input/output interfaces, and various sensors. The video game will be an abstraction of the box's interior, allowing the player to interact with components of the box while also requiring to solve software only components.

The goal likewise will be two fold. The user should expect a story to unfold as they progress through the puzzle, as well as creating a unique experience where physical components affect a software world and a software character should be made to feel real through the outputs created by the puzzle box.

# Development

Development of this project will be completed in 4 major stages.

1) Creating the ground work. To prototype this project, I intend to take advantage of the various sensors and inputs available on a common smart phone and design a simple unity input reader for these devices. The end goal of this stage will to have an android game which displays detailed information relating to light detection, orientation, acceleration, as well as reading button inputs and displaying these readings in real time on the phone screen.

2) Creating the two way input/output channel. Once an input reader is functionally running native on the android phone, the next step will be to bridge the gap between external interface and a video game run on a PC. A two-way communication system will be opened so that raw input can be fed from the phone into the PC and displayed on a monitor, and then the PC will analyze the raw input and produce an image to display on the phone screen. The completion of this stage will indicate the project as ready for puzzle development.

3) A simulation of a puzzle box rendered in the phone. As fun as purchasing various input components, wiring and unwiring devices, and possibly prototyping various box designs could be, this stage provides two useful benefits. First it will allow for cheaper testing of the final physical puzzle box as the devices can be simulated and then much more easily integrated/removed during development. Second is that I do not expect the final puzzle box to have any proper way to be circulated. While I can issue out 3D print files, part lists and assembly instructions, a game should be fun and unrestricting. The final project presents a great barrier to entry and if possible I'd like to provide a means to trial the experience without requiring a great investment.

4) Final development of the puzzle box. At this stage the box itself will be simulated as a 3D model both to layout out the game space for the video game component, and for a visual representation displayed on the android app. At this point a part list should already be prepared, the 3D model of the box should be made to export as a printable file or a CNC cutting schematic, and a true device should be able to be constructed.
