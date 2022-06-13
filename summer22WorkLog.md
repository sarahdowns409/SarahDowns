---
layout: default
---

<center> <h1>Summer 2022 Worklog </h1></center>

## Important Summer Dates

- <b> June 15 </b>: NGA Site Visit
- <b> June 22 </b>: SDSC CIML Prep Day
- <b> June 27 - June 29 </b>: SDSC CIML
- <b> July 6 - July 10 </b>: Phi Mu National Convention (Sarah no work)
- <b> July 25 </b>: DFD Abstracts due
- <b> August 6 - August 20 </b>: Tour de Mont Blanc (Sarah no work)

## May 9 - May 13

- Downloaded VisIt to PC (wasn't on this one since my old computer broke) and set-up to use.
	- Update: Not enough room on my PC, but it looks like the most recent version of VisIt runs on Mac, so trying that instead
	- Update: having trouble downloading the viz-IB3d file to get coral data. Might need to put on external drive from my old laptop or find a way for Matea to resend if it keeps not working
	- Update: to use VisIt on Mac, need to cd into the folder holding data that you want to use and then run terminal using the command `/Applications/VisIt.app/Contents/Resources/bin/visit`
- Created work-log for the summer
- Started looking into created website using GitHub. Following the [Github Pages Tutorial](https://lab.github.com/githubtraining/github-pages). Will come-back to.
- Completed SMART orientation
- Continued working on VTK conversion to MATLAB. Stuck on figuring out the pattern to attach points to cells
- Met with Matea to discuss summer goals and next steps

## May 16 - May 20

- Took a break to recover from semester -- no work

## May 23 - May 27

- Continuing work on VTK conversion
	- End of day Monday-- Works for some files, but not all. Need to figure out issue
	- Update: issue was with how points were attached to cells-- fixed the way this is down and now it appears to work better
	- End of day Tuesday-- Works properly for all VTK files in one folder, want to make it so it loops through each folder next. Also need to figure out how to make mesh out of points (currently doing this on small scale for each file, not sure if I can just make a larger version of this or if there is something more efficient
- Attended Kleckner lab meeting to listen to Mahdi talk about his work on chaos-- will read more about and talk to Matea to see if we want to apply this to corals
- Think I got code working to loop through all folders and files and find the VTK information
- Started working on reading Applied Solid Mechanics book again
	- Had to restart because it had been so long
	
## May 31 - June 3

- Continued reading Applied Solid Mechanics
- Brief meeting with Matea to talk about vtk extraction code
	- Code should sort data so that a points neighbors are the points directly above and below it in the array.
	
## June 6 - June 10

- Fixed vtk conversion code so that it sorts data
- Figured out how to create GitHub website
	- Spent a while setting page up and putting CV and about me on website
- Met with Matea to talk about next steps
	- vtk extraction code should work with what she has
	- Next: look into high order interpolation schemes that are dependent on how far away points are (3rd order, weighted)
		- Needs to work on non-uniform grid
		- Make sure that all weight add up to 1
		- Also needs to be divergence free
		
## June 13 - June 17

- Looking for papers on new implementation scheme. 
	- <i> Irrotational or Divergence Free Interpolation </i>: Don't think that I'll be able to implement this paper, especially since it doesn't really go into how the scheme is devised
	- <i> An Immersed Boundary Method with divergence-free velocity interpolation and force spreading </i>: Requires that we know mesh width, need to find a method that does not depend on mesh and is only based on distance
	- <i> A novel interpolation-free sharp interface immersed boundary method </i>: Gets rid of need for interpolation altogether, but requires implementing an almost new method
	- <i> An immersed boundary method for nonuniform grids </i>: Don't think this fits what I want, but unclear. Could keep in mind as a backup option
	- <i> Radial basis function (RBF)- based interpolation and spreading for the Immersed Boundary Method </i>: Think that this method is what I want. Mesh-free meaning that weights are calculated only on the Euclidean distance. Gives condition to guarantee that it is divergence free. Not sure how hard it will be to implement, but will start here. 

## June 20 - June 24

- 

## June 27 - July 1

- 

## July 5 - July 8

- 4th of July and Phi Mu National Convention -- no work

## July 11 - July 15

- 

## July 18 - July 22

- 

## July 25 - July 29

- 

## August 1 - August 5

- 