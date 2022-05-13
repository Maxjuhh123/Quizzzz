# Starting template

This README will need to contain a description of your project, how to run it, how to set up the development
environment, and who worked on it. This information can be added throughout the course, except for the names of the
group members. Add your own name (do not add the names for others!) to the section below.

## Description of project

## Group members

| Profile Picture | Name | Email |
|---|---|---|
| ![Max de Groot](https://gitlab.ewi.tudelft.nl/uploads/-/system/user/avatar/5033/avatar.png?width=96) | Max de Groot | M.R.degroot-1@student.tudelft.nl |
| ![Demetra Carata](https://secure.gravatar.com/avatar/1872d0d272df591c5e120f0574cf657f?s=192&d=identicon&size=96&width=96) | Ioana Demetra Carata Dejoianu | I.D.CarataDejoianu@student.tudelft.nl |
| ![Jakub Kontak](https://gitlab.ewi.tudelft.nl/uploads/-/system/user/avatar/4493/avatar.png?width=96&size=50) | Jakub Kontak | J.Kontak@student.tudelft.nl |
| ![Daniël Ravensbergen](https://gitlab.ewi.tudelft.nl/uploads/-/system/user/avatar/5010/avatar.png?width=96&size=50) | Daniël Ravensbergen | D.G.S.Ravensbergen@student.tudelft.nl |
| ![Lauri Kesküll](https://gitlab.ewi.tudelft.nl/uploads/-/system/user/avatar/4943/avatar.png?&width=96&size=96) | Lauri Kesküll | L.Keskull@student.tudelft.nl |
| ![Alexandra Carutasu](https://gitlab.ewi.tudelft.nl/uploads/-/system/user/avatar/4756/avatar.png?width=96&size=50) | Alexandra Carutasu | A.Carutasu@student.tudelft.nl |

## How to run it

You should download the game. You should have a stable internet connection in order for the game to work properly.
The game doesn't look that well on smaller screen sizes (like most macbooks) so a resolution of atleast 1920 x 1080 is recommended.

In order for the game to work you should also download the folder containing the activities in the following way:

If there is already an activities folder in the project folder you can skip steps 1 and 2
1. Go to https://gitlab.ewi.tudelft.nl/cse1105/2021-2022/activity-bank/-/releases
2. Get the zip folder containing activities and the activities.json file, unzip it and move it to the project file.
3. Open the project in an IDE (we use IntelliJ IDEA)
4. Make sure you have javaFX downloaded
5. Edit the run configuration of the following file: client/src/main/java/client/Main.java by adding the path to the JavaFX runtime folder as a paramater, it is also recommended to rename the comfiguration to something like "Client". This is what the configuration should look like:
![image](https://user-images.githubusercontent.com/97608160/168282222-cf73e078-aae2-42fe-b735-722f2e07f97a.png)
You can also enable "Allow multiple instances" so you can play multiplayer on one device.
6. Now run the following file to start the server: server/src/main/java/server/Main.java
7. If you then run the file mentioned in step 5, the application should launch.
8. Now you can import the activity bank (the activities.json file from step 2) from the admin panel. The game should be playable now.

You should only have to do this once to get the activities into the server as they are stored in the database after importing.

If launching a game still doesn't work, try deleting quizzz.mv and other .db files from the project folder.

## How to contribute to it

We adhere our code style to that of https://google.github.io/styleguide/javaguide.html

Follow this guide to set up your IDE accordingly.

1. Install the plugin
    - Go to File -> Settings -> Plugins
    - Select the Marketplace tab
    - Search for CheckStyle-IDEA and install it
    - Press Restart IDE
    - Press Restart
2. Configure checkstyle
    - Go to File -> Settings -> Tools -> Checkstyle
    - Make sure you have Checkstyle version 9.3
    - Set the Scan Scope to All files in project
    - Enable 'Treat Checkstyle errors as warnings'
    - Click the + Symbol to add a configuration file
    - Enter a Description (e.g. Custom checkstyle rules)
    - Press Browse
    - Select the checkstyle.xml file in the root of the project
    - Enable 'Store relative to project location'
    - Press 'Next'
    - Press 'Next' again
    - Press 'Finish'
    - Activate the newly added checkstyle rules by pressing the checkbox of the corresponding configuration file
    - Press 'Apply' to save the changes
3. Update the code style of the editor
    - Go to File -> Settings -> Editor -> Code Style
    - Select Project as scheme
    - Press the settings icon
    - Press 'Import Scheme'
    - Press 'CheckStyle Configuration'
    - Choose the checkstyle.xml file that is in the root of the project
    - Press 'OK'
    - Press 'Apply'
4. Automate reformatting (recommended)
    - Go to File -> Settings -> Tools -> Actions on Save
    - Enable the following actions
        - Reformat code
        - Optimize imports
        - Rearrange code
    - Press Apply

## Copyright / License (opt.)

OOPP Group No. 17
