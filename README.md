# A small pizza slice for educational purposes
Follows [this guide](https://realmdex.com/index.php?threads/how-to-setup-your-new-private-server-using-skillys-educational-source.39/), based on [Skilly's Educational Source](https://www.mpgh.net/forum/showthread.php?t=1523250) updated for 2024.

## Setup
1. Download [IntelliJ IDEA Ultimate 2024](https://www.jetbrains.com/idea/download/?section=windows) (30-day free trial). Run it, click plugins, and install the Flash/Flex plugin.
2. Download [AIR SDK](https://airsdk.harman.com/download). This is needed to compile the client.
3. Download [Flash Player 32](https://archive.org/details/flashplayer_32_sa_202104) and place it in `C:/Users/USERNAME/flashplayer_32_sa_debug.exe` (notice the added `_debug`) in the file name.
4. Open the `realm-server-master` folder in IntelliJ and click the play button to run it. I use VSCode instead of IntelliJ for this.
5. Open `realm-client-master` in a separate IntelliJ window. Click menu in top left > Project Structure. In the Project tab, edit the SDK and locate the AIR SDK you downloaded in step 2. Set language level to SDK default.
6. In the Modules tab, click WebMain (app) > Dependencies and select the AIR SDK.
7. Click the green play button at the top to run the code in debugging mode. 

> If you get an error regarding flash player, you'll need to find the project configuration 

> If you get an error for the `LegendsList..` file, right click and Jump To Source, then hover over the faulty code (red underline), click see options, and select the option named something like "cast type".

### Other resources
https://github.com/Devwarlt/LoE-Realm-NC-2/blob/production/HowToSetup.md