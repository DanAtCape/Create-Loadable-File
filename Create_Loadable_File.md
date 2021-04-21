# Creating A Loadable File for Bonsai Brain 
To train a Bonsai brain with VP Link, a loadable file must be generated. This loadable file is a ZIP file with files VP Link needs to run a simulation. Below are steps describing how to create a loadable ZIP file.<br>
If you already have a loadable file, see docco for the next step: [Creating Bonsai Brain](./Create_Bonsai_Brain.md).<br>

**1.) Access VP Link via Azure**<br>

*... More goes here - how to access VM ...*

Once on the machine, start VP Link using the VP3 Control Panel shortcut:<br>

![VP3 Shortcut](/images/Capetest_VP3ControlPanelShortcut.png)<br>

Open the Livecode stack that has the *Bonsai Tags* page (e.g., SimpleTank.rev). Then load the VP Link tag database for the simulation to be used on the Bonsai Brain.<br>

**2.) Select Tags For The Brain**<br>

Go to the *Bonsai Tags* page:<br>

![Bonsai Tags page](/images/Capetest_BonsaiTags_SimpleTank.png)<br>

The *selection* field on the left is for listing tags in the current simulation that will be selected to use for the brain. The top-right field is for tags the Brain will try to control (**State Tags**), and the bottom-right is for tags the Brain will manipulate in order to control the state tags (**Action Tags**).

To get tags in the simulation listed in the left field, use the *Search* window in VP Link to select the desired tags, then use the **Actions** -> **Copy Spreadsheet** menu to copy tags in the Search window to the clipboard.<br>

![Copy Spreadsheet](/images/Capetest_BonsaiTags_CopySpreadsheet.png)<br>

Then click the **Paste Spreadsheet** button on the *Bonsai Tags* page (see screenshot above) to copy tags from the clipboard to the selection field.<br>

Once tags are available, select a tag and click the **Add tags to State** or **Add tags to Action** button to place the tag in the appropriate list (state or action).<br>

**3.) Build Bonsai Loadable**<br>

Note the *Loadable SubDir:* field next to the button.<br>

![Loadable SubDir](/images/Capetest_BonsaiTags_LoadableSubDir.png)<br>

This is to use separate folders for each loadable that is created. Using different sub-directories will keep different brain simulations separate. Optionally choose a sub directory name, then click the **Build Bonsai interface** button. If no folder exists with the SubDir name, there will be a couple dialog windows to create the folder.<br>
*... Is this dialog (TWO dialogs) necessary ...?*<br>

![Build msg 1](/images/Capetest_BonsaiTags_BuildMsg.png)<br>

Then click the **Create Bonsai Loadable** button. To show the folder where the loadable is located, click the **Show Loadable** button. The *ZIP* file is the loadable needed as input to the Bonsai Brain.<br>

![Loadable ZIP folder](/images/Capetest_BonsaiTags_LoadableInFolder.png)<br>

