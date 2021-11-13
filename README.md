				   _____          __                          .__  __
				  /  _  \  __ ___/  |_  ____             ____ |__|/  |_
				 /  /_\  \|  |  \   __\/  _ \   ______  / ___\|  \   __\
				/    |    \  |  /|  | (  <_> ) /_____/ / /_/  >  ||  |
				\____|__  /____/ |__|  \____/          \___  /|__||__|
				        \/                            /_____/

A simple bash script that automatically pushes your code to Github without typing out all the steps. It saves me
a lot time and I hope it can help you too. Works on any machine capable of running bash shell. I plan on adding more
features in the future so stay tuned! Thanks for checking it out!

	Instructions (Linux)
	1.Clone the repo to your local drive and change into that newly created directiory.
	2.Use "chmod +x autogit " to make it executable.
	3.Use "sudo nano ~/.bashrc" and scroll to the very bottom (or whatever text editor you like to use).
	4.Add in "export PATH=~/Auto-git:$PATH " to make the current user able to execute the bash script from
	  any directory (no quotations). You can replace the path with wherever directory you cloend the repo into.
	5.Save and exit with ctrl+x , 'y' , and enter to accept the changes.
	6.Done! Now the bash script should work by calling it with "autogit [flag] [input]". Refer to "autogit -h"
	  to find out more about different flags. (A retart of terminal may be required)

	Instructions (MacOS)
	1.Clone the repo to your local drive and change into that newly created directiory.
	2.Use "chmod +x autogit" to make it executable.
	 *Note: On MacOS there will be no .bashrc file. When Mac terminal opens up, it reads these files in a
	  different order and will not read the .bashrc unless we do other steps. Instead to make this easier
	  we will be making a .bash_profile file.
	3.Use "sudo nano ~/.bash_profile " to create a blank .bash_profile file and use "export PATH=~/Auto-git:$PATH"
	  (if your cloned directory is in a different location then change the path 
	  "export PATH=<insert your path here>:$PATH"
	4.Save and exit with ctrl+x , 'y' , and enter to accept the changes.
	5.Done! Now the bash script should work by calling it with "autogit [flag] [input]". Refer to "autogit -h"
          to find out more about different flags.Done! Now the bash script should work by calling it with "autogit [flag] [input]". Refer to "autogit -h"
          to find out more about different flags. (A restart of terminal may be required) 

	example: autogit -m "Thanks Autogit!"
	*performs
		- git add .
		- git commit "Thanks Auto-git!"
		- git push origin main

 
UPDATE![11/4/21]: Just added the create a repository feature. It just calls the gh tool (Github CLI) to make a new 
repository and initializes it so that the repo is ready to use right away. It saves me a lot of time because now I 
rarely have to leave my keyboard!! Refer to Github CLI documentation for instructions on how to download Github CLI
on your system. I plan on adding more in the future so stay tuned!


