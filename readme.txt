DayZ Chernarus Chernogosk Trader Ships Custom Structure Json File For Console and PC Instructions & Terms Of Use

ORIGINAL MOD BY N10248 = A BIG THANKS TO HIM & Reaper 1of4 WHO CREATED IT!

https://steamcommunity.com/sharedfiles/filedetails/?id=3022530513

(See his instructions at above page for how to install structure as a trader base).

Spawns a number of large ships and other structures around the docks in Chernogorsk on Chernrus which is on the Docks in Svetlojarsk on Chernarus.

Limited Testing on PC Chernarus Local Server DAYZ Version 1.22 Aug 23.

Json Created by @scalespeeder. Please report bugs & errors to scalespeeder@gmail.com with screenshots.

If you'd like to edit & customize the structures, simply load "tradership.dze" into DayZ Editor.

Many Thanks To Inclement Dab for his amazing DayZ Editor that makes this all possible: https://steamcommunity.com/sharedfiles/filedetails/?id=2250764298

TERMS OF USE
THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS
OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN
AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH
THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

Using these modded json files and instructions could break the functioning of your DAYZ server, requiring a reinstall that would wipe
all player progress.

Using these modded files neccessitates increased regular restarts to prevent server crashing.

It is suggested you thoroughly test your server after applying these files to ensure proper
functioning of your server.

I always recomend you validate your files at: https://www.xmlvalidation.com/ and https://jsonformatter.curiousconcept.com/

Instructions:

Click the "Code" button and "Download Zip" on the Github Repository and extract the files on your local PC for access.

Stop your server.

Ensure your DayZ Server has activated the cfggameplay.json. For console users on Nitrado Servers, go to "General Settings" on your server and tick "Enable cfggameplay.json".

On PC Servers add the following line to your serverDZ.cfg:

enableCfgGameplayFile = 1;

(On some PC servers, including Nitrado, the serverDZ.cfg is "hidden", so you need to enable "expert mode" in settings,
then go to "expert settings", which is the serverDZ.cfg. Stop the server before making changes this way.)

Upload "trader-ship.json" from the extracted files to inside the "custom" folder of the mission directory on your server.
(If you haven't got a "custom" folder, create one.)

Open the cfggameplay.json file in the correct mission file for your server and look for the "objectSpawnersArr" line.

This file tells your server to access your custom file.

Edit it to look like this: 

	"objectSpawnersArr": ["custom/trader-ship.json"],	
	
If you already are calling custom jsons to spawn items or buildings, seperate the files like this:

	"objectSpawnersArr": ["custom/trader-ship.json","custom/anotherfile.json","custom/differentfile.json"],
	
Save your changes & upload if you need to.

To add loot to the new structures, add the below XML code snippet to your servers mapgrouppos.xml file, at the top, below <map>

<!--trader ships loot-->
	<group name="Land_Ship_Big_FrontA" pos="6888.490234 12.000000 2600.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_Ship_Big_FrontB" pos="6886.180176 10.500000 2619.899902" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_Ship_Big_BackA" pos="6884.950195 12.000000 2655.399902" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_Ship_Big_BackB" pos="6885.500000 10.500000 2675.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_Ship_Big_Castle" pos="6885.299805 20.650000 2663.600098" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Bonfire" pos="6885.000000 21.000000 2670.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Tisy_RadarPlatform_Mid" pos="6885.299805 -7.550000 2641.500000" rpy="0.000000 9.999997 0.000000" a="90"/>
	<group name="StaticObj_Tisy_RadarPlatform_Mid" pos="6885.299805 -7.550000 2623.500000" rpy="0.000000 9.999997 0.000000" a="90"/>
	<group name="StaticObj_Tisy_RadarPlatform_Mid" pos="6885.299805 -7.550000 2597.600098" rpy="0.000000 9.999997 0.000000" a="90"/>
	<group name="Land_Pier_Crane_A" pos="6866.500000 8.300000 2574.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Pier_Crane_B" pos="6869.500000 21.200001 2578.199951" rpy="0.000000 0.000000 -45.000000" a="135"/>
	<group name="Land_Pier_Crane_A" pos="6867.500000 8.300000 2706.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Pier_Crane_B" pos="6872.200195 21.200001 2703.000000" rpy="0.000000 0.000000 30.000000" a="60"/>
	<group name="Land_Container_1Aoh" pos="6877.899902 11.800000 2587.000000" rpy="0.000000 0.000000 21.999996" a="68"/>
	<group name="Land_Container_1Bo" pos="6867.000000 4.100000 2585.000000" rpy="0.000000 0.000000 12.000000" a="78"/>
	<group name="Land_Castle_Stairs" pos="6867.100098 0.650000 2648.500000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Wall_CncBarrier_Block" pos="6876.600098 6.600000 2649.500000" rpy="-179.999954 0.000000 90.000000" a="0"/>
	<group name="Land_Roadblock_Table" pos="6878.399902 7.900000 2643.600098" rpy="0.000000 0.000000 45.000000" a="45"/>
	<group name="Land_Roadblock_Table" pos="6886.000000 7.900000 2643.399902" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Roadblock_Table" pos="6886.000000 7.900000 2653.399902" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Roadblock_Table" pos="6891.700195 7.900000 2652.600098" rpy="0.000000 0.000000 45.000000" a="45"/>
	<group name="Land_Roadblock_Table" pos="6891.600098 7.900000 2644.000000" rpy="0.000000 0.000000 -45.000000" a="135"/>
	<group name="Land_Roadblock_Table" pos="6878.399902 7.900000 2653.000000" rpy="0.000000 0.000000 -45.000000" a="135"/>
	<group name="Land_Mil_GuardShed" pos="6836.500000 3.500000 2659.100098" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Wall_FenR_3" pos="6822.399902 4.200000 2662.500000" rpy="0.000000 0.000000 64.999992" a="25"/>
	<group name="StaticObj_Wall_FenR_3" pos="6824.299805 4.200000 2660.000000" rpy="0.000000 0.000000 -159.999954" a="-110"/>
	<group name="Land_Ship_Big_FrontA" pos="7137.000000 24.400000 2614.000000" rpy="0.000000 0.000000 142.999954" a="-53"/>
	<group name="Land_Ship_Big_FrontB" pos="7151.500000 22.900000 2627.800049" rpy="0.000000 0.000000 142.999954" a="-53"/>
	<group name="Land_Ship_Big_BackA" pos="7178.899902 24.400000 2650.000000" rpy="0.000000 0.000000 142.999954" a="-53"/>
	<group name="Land_Ship_Big_BackB" pos="7194.899902 22.799999 2661.300049" rpy="0.000000 0.000000 142.999954" a="-53"/>
	<group name="Land_Ship_Big_Castle" pos="7185.700195 33.049999 2654.600098" rpy="0.000000 0.000000 142.999954" a="-53"/>
	<group name="Land_Misc_Scaffolding" pos="7166.000000 8.600000 2655.409912" rpy="0.000000 0.000000 53.000000" a="37"/>
	<group name="Land_Misc_Scaffolding" pos="7136.500000 8.600000 2632.000000" rpy="0.000000 0.000000 48.000004" a="42"/>
	<group name="Land_Tenement_Big" pos="6779.500000 26.000000 2513.199951" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Garbage_Pile4" pos="6787.500000 3.100000 2503.100098" rpy="0.000000 0.000000 10.000000" a="80"/>
	<group name="StaticObj_Platform2_Stairs_30" pos="6779.000000 3.900000 2525.000000" rpy="0.000000 0.000000 -179.999954" a="-90"/>
	<group name="StaticObj_Platform2_Stairs_30_WallR" pos="6780.250000 3.900000 2524.100098" rpy="0.000000 0.000000 -179.999954" a="-90"/>
	<group name="StaticObj_Platform2_Stairs_30_WallL" pos="6777.799805 3.900000 2524.100098" rpy="0.000000 0.000000 -179.999954" a="-90"/>
	<group name="StaticObj_Road_Sidewalk_Stairs" pos="6778.270020 7.060000 2516.899902" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Ship_Big_FrontA" pos="7059.000000 13.000000 2207.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Ship_Big_FrontB" pos="7039.100098 11.500000 2204.649902" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Ship_Big_BackA" pos="7005.000000 13.000000 2203.399902" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Ship_Big_BackB" pos="6985.299805 11.500000 2204.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Ship_Big_Castle" pos="6996.700195 21.650000 2203.750000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Tisy_RadarPlatform_Mid" pos="7027.100098 -6.420000 2204.000000" rpy="0.000000 9.999997 90.000000" a="0"/>
	<group name="StaticObj_Tisy_RadarPlatform_Mid" pos="7019.000000 -6.420000 2204.000000" rpy="0.000000 9.999997 -90.000000" a="-180"/>
	<group name="StaticObj_Tisy_RadarPlatform_Mid" pos="7061.299805 -6.420000 2204.000000" rpy="0.000000 9.999997 -90.000000" a="-180"/>
	<group name="Bonfire" pos="6990.500000 21.500000 2204.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Ship_Big_FrontA" pos="7859.000000 13.000000 2207.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Ship_Big_FrontB" pos="7839.100098 11.500000 2204.649902" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Ship_Big_BackA" pos="7805.000000 13.000000 2203.399902" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Ship_Big_BackB" pos="7785.299805 11.500000 2204.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Ship_Big_Castle" pos="7796.700195 21.650000 2203.750000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Tisy_RadarPlatform_Mid" pos="7827.100098 -6.420000 2204.000000" rpy="0.000000 9.999997 90.000000" a="0"/>
	<group name="StaticObj_Tisy_RadarPlatform_Mid" pos="7819.000000 -6.420000 2204.000000" rpy="0.000000 9.999997 -90.000000" a="-180"/>
	<group name="StaticObj_Tisy_RadarPlatform_Mid" pos="7861.299805 -6.420000 2204.000000" rpy="0.000000 9.999997 -90.000000" a="-180"/>
	<group name="Bonfire" pos="7790.500000 21.500000 2204.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>

<!--end of trader ship loot-->

Restart your server and the new objects will appear immediatly.

Thanks, Rob.