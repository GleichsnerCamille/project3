The included files are only for the build they are not the actual coding assets themselves.

Programs Used: 
Unity 
Visual Studio Preview for C# scripts

Keep in Mind: 
- I didn't have much experience with Unity in terms of mechanical coding. Basic 
	platforming and snake. I wanted to test myself to learn even basic forms 
	of mechanical coding and selected: double jumping, wall jumping, wall sliding, 
	wall climbing, reverse gravity, and color based disappearing/appearing mechanics. 
- I didn't have as much time as I would have liked to have had. Alot of time was teaching myself 
	in the two weeks I was given how to make these mechanics in C# and proper use them in Unity. 
	I also knew I wanted to remake the controls I used for an earlier extremely basic platforming game
	I made. Which meant new animation cycles, and messing with timings and needing to remember to click on	
	certain unity settings. I also needed to make three new animation cycles for both the player and the
	enemies based on RGB coloring, which at first felt like an odessy of a task, but Syncing the animations
	made the process much easier. 
- I didn't make a menu as I felt this project was showing how much I could learn by myself for more complex mechanics
	then moving, jumping, respawning, killing enemies, switching the level, and camera movement. I felt a menu was 
	really just a waste of time when there were only two options: Play and Exit.
- I didn't include any music as I wasn't sure of copyright laws and fair use, and felt I would rather just play it safe
and not add in music over all. 


Issues:
- Dying in reverse gravity had... complications for simple design
	I opted for a jank but technically effective system to negate the speed shift.
	It will look like the game is glitching, just give it at most 6 to 7 seconds
	and the character will be probably respawned in normal gravity
- I am not an animator, nor am I a digital artist. I spent way too much time messing
	with the player character's animations so at least the player character felt good
	and semi responsive. This took me 2 days to manage and mess with timings, animation
	switches, and of course drawing out the sprites. By the time I got to wall climbing 
	I didn't have the time to be animating anything. 
- Walling climbing feels awkward to use, and was not the bane of my existance I was expecting 
	it to be. The climbing was decent but with no animation cycle it feels weird, but jumping?
	Well I spent a day alone trying to get the jumping to propel at an angle, which result in 
	more lost time. 
- Double Jumping has a different jumping style than base jumping, and is refilled when in contact range of
	any ground object. So you can, and may notice, if you manipulate it right you can in theory even triple jump. 
- Turning off a color sometimes results in certain things breaking? I was unable to determine why as most often
	they woould work correctly but from time to time things will suddenly not be where they were meant to be. 
	for nearly no rhyme nor reason. I assume it has something to do with some gravity scale delay with my scripts 
	but I can't make up for my code taking a second too long to complete before an object freezes in place in the
	wrong area without spending more time I just didn't have.




Notes
- Reverse gravity took longer than I had expected. There were unique complications such as jump force 
	actually not being complex. I had assumed I would need a downward jump force and that actually made 
	things worse. Which served as a lesson to test before editing scripts for mechanics. What became the issue
	was ground detection. You can read the "Notes" section of this document for more information on that. However,
	the animations weren't how I wanted them, and the the player could run mid air when reversed. Maybe it wasn't 
	important, but it bothered me and I couldn't even sleep knowing it was not how I wanted it to look. I ended up 
	spending 2 days on reverse gravity mechanics in total mostly around how everything looked and felt. I had to make two seperate 
	systems of ground detection, as the system I made for reverse gravity broke my double jumping. Depending on if the blue was reveresed 
	or normal gravity determines what system of ground detection is used. 
- Double jumping was more... sensitive than I expected. I played with it for several hours,until I decided I need to just make a second
	system of jumping that replaces the main jump when double jump is active. 
- My proudest moment was becoming frustrated when I realized making objects disappear for each of the three RGB colors would take three
	scripts, adn appearing was three more. I hated this, and decided to merge them based on public string inputs and switch 
	statements for color and mechanic. I then realized I also need to make the colliders, both box and circle, also appear/disappear.
	Which would have been yet more scripts. So instead, I wrote one massive script with four tiers of switch statements. It hurt to witness,
	but made my life so much easier. It also allowed for more flexability with mechanic design. This isn't impressive, more just realizing
	I could make it all based on options and speed up the level building process.  
