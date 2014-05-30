Ruby Ship
=========

Portable ruby environment on any platform, with any version of MRI Ruby! No need to install Ruby on a computer to use it any more! 

The goal of Ruby Ship is to have a single folder which is portable on all platforms. 

This is very usefull when developing ruby applications when your target audience does not have ruby installed, and you do not want to bother with installing ruby for them.

With Ruby Ship you can copy the entire folder into your project and use the wrappers supplied to make any ruby script run.

Ruby Ship comes with tools to compile your favourite Ruby version too! This way, you are not stuck with the binaries that Ruby Ship happens to come with. 

![Ruby Ship](/image/ruby_ship.png?raw=true)


## Install:

- Step 1: Download this repository

- Step 2: Put the bin folder wherever you want it.

- Step 3: Use the ruby_ship wrappers as you would use the normal ruby command.

- Step 4: Party, Celebrate, and Contribute to Ruby Ship!


## Usage:

in a command line environment:
```
path/to/bin/ruby_ship.sh [your normal ruby args]
```
```
path/to/bin/ruby_ship.bat [your normal ruby args]
```

Example

path/to/bin/ruby_ship.bat -e "puts 'Ruby Ship works!'"



## Current pre-bundled versions of ruby:

- Windows: 2.0.0p481
- OSx: 2.1.2p95
- More platforms coming. 

## Building other ruby version

Getting a new version of ruby is super-easy! Go to https://www.ruby-lang.org/en/downloads/ and download the **tar.gz** you desire. Then run the following command. 

```
#For *nix
/tools/ruby_ship_build.sh path/to/source/ruby-X.Y.Z.tar.gz
```
```
::For windows
/tools/ruby_ship_build.bat path/to/source/ruby-X.Y.Z.tar.gz
```

Thats it! After this finishes you will have a new 'platform'\_ruby.sh ruby wrapper in your ruby\_ship/bin/ folder.

Now you can use your ruby_ship.sh/.bat with your newly compiled ruby version! The best part is: You can copy this environment wherever you want, and it will still work! Ship it with your product, place it on a USB, or do whatever you want with it! No need to install ruby ever again!

Note: You must compile ruby using ruby\_ship\_build on the platform you want to use this on, but only once :)

## License:

MIT

## TODO:

- Binary for all platforms (compiling from source)
- Make compile-script for each platform so anyone can update ruby version if needed. (should be easy)
- Have the compile script also generate the wrapper to take into consideration changing ruby versions.
- Make wrappers for bundle, gem, etc. (could be hard)