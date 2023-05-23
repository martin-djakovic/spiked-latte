## How to install
NOTE: The installation guide is for Visual Studio ONLY! If you want to use a different IDE/editor, or compile this code on Linux or MacOS, this guide doesn't apply

 1. Make sure you have C++ installed in Visual Studio - https://irendering.net/how-to-install-c-and-c-support-in-visual-studio/
 2. Download the necessary dependencies (SDL2, SDL2_image and SDL2_ttf) from the following links: https://github.com/libsdl-org/SDL/releases/tag/release-2.26.5, https://github.com/libsdl-org/SDL_image/releases/tag/release-2.6.3, https://github.com/libsdl-org/SDL_ttf/releases/tag/release-2.20.2. Make sure to download the `VC` file. Extract the downloaded files, and place the extracted files to a location that you'll remember (don't leave it in Downloads!)
 3. Follow the guides here to add the necessary libraries to your project: https://lazyfoo.net/tutorials/SDL/01_hello_SDL/windows/msvc2019/index.php, https://lazyfoo.net/tutorials/SDL/06_extension_libraries_and_loading_other_image_formats/windows/msvc2019/index.php
 4. If you installed the libraries according to the guide listed above, you will have to remove the `SDL2/` prefix in all the `#include` paths in the project
 5. In the `common.hpp` file, change all the variables relating to the file paths of game assets, to the absolute path of the game assets on your computer (e. g. change `"assets/player.png"` to `"C:\\Users\\John\\OneDrive\\Documents\\Visual Studio 2022\\Projects\\Spiked-Latte\\assets\\player.png"`

That's it! You should now be able to compile the code and run it!
