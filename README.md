# The Ur-Quan Masters MegaMod
A fork of The Ur-Quan Masters that continues the HD mod with a veritable smorgasbord of extra features.

## Changes from the original

A full list of changes and features can be found on the [Main site](http://megamod.serosis.net/Features).

And the current changelog can be found in the repository: [Changelog](https://github.com/Serosis/UQM-MegaMod/blob/master/MegaMod%20Changelog.txt)

## Motivation

This project exists out of my love for Star Control II and The Ur-Quan Masters project. Fiddling with the code as a hobby to try and expand my skill as a programmer.

## Windows Installation

Open up the installer, pick your optional content, wait for all of it to download and install, then play!

## MacOS X Installation

Mount the .dmg file and copy the app to your Applications folder.

## Building Yourself

### Windows

#### Visual Studio 
I've made the process super easy for Windows, as long as you have Visual Studio 2008 or Visual Studios 2015-2019. Just load up the solution file and compile away.
For Visual Studio 2008 the solution file is under `build/msvs2008` for Visual Studios 2015-2019 the solution file is under `build/msvs2019`

#### MinGW

Start MSYS and `cd` to the UQM-MegaMod directory then execute this command:  

`./mingw.sh uqm`

Or if you want to do it manually execute these commands: 

`export C_INCLUDE_PATH=$PWD/dev-lib/MINGW/include`  
`export LIBRARY_PATH=$PWD/dev-lib/MINGW/lib`  
`export PATH=$PATH:$PWD/dev-lib/MINGW/bin`  
`./build.sh uqm`  

When executing the helper script or last command in the manual method you'll come to a configuration screen where you can select a few developer-centric options.  
Just hit `enter` and UQM will start building. It'll take awhile and you'll see a few scary warnings but everything *should* build fine.

### Other Platforms
You'll have to gather all of the necessary dependencies and hope for the best.

#### Tips

For all platforms when building from commandline you can use the command `-j#` to invoke multi-threaded performance to dramaticly speed up build time.  
Example: If you're running on a Ryzen 7 2700x you can use the command like so `./build.sh -j16 uqm` to take advantage of all your threads.

This also works with the MinGW helper script in the same manner: `./mingw.sh -j16 uqm`

## Contributors

Me (Serosis), SlightlyIntelligentMonkey, and Ala-lala

The main menu music for the MegaMod is brought to you by Saibuster A.K.A. Itamar.Levy: https://soundcloud.com/itamar-levy-1/star-control-hyperdrive-remix, Mark Vera A.K.A. Jouni Airaksinen: https://www.youtube.com/watch?v=rsSc7x-p4zw, and Rush AX: http://star-control.com/fan/music.php.

And the default Super Melee menu music is by Flashy of Infinitum.

## License

The code in this repository is under GNU General Public License, version 2 http://www.gnu.org/licenses/old-licenses/gpl-2.0.html

The content in this repository is under Creative Commons Attribution-NonCommercial-ShareAlike, version 2.5 https://creativecommons.org/licenses/by-nc-sa/2.5/
