Link 

For macOS:(RAxML-NG v1.2.2)
If you're on a macOS system (either Intel or Apple Silicon ARM), the easiest way to install RAxML-NG is by using the pre-compiled binary. You don’t need to build it from scratch. Here's what you can do:

1.Download Pre-Compiled Binary for macOS:

Go to the release section of RAxML-NG: RAxML-NG Releases


2. Download the macOS binary (either x86 or ARM based on your system architecture).

Extract the ZIP File:

Once the binary is downloaded, unzip it and place it in a directory where you want to run it from.



3. Run RAxML-NG:

Open your terminal and navigate to the directory where the RAxML-NG binary is located.

Run commands like ./raxml-ng to use the program for phylogenetic analysis. For example:

 ./raxml-ng --search1 --msa H3_Codon_Alignment.fas --model GTR+G

_______________________________________________________________________________________________________________________________________________

ERROR: SECURITY ISSUES TROUBLESHOOT
The error you're encountering is a common security warning on macOS when trying to open applications that are downloaded from the internet or aren't from an identified developer.
Here's how to bypass this security feature and open the RAxML-NG binary:

Steps to Open RAxML-NG on macOS:
1. Go to System Preferences:
Click on the Apple menu (top left corner) and select System Preferences.

Then, select Security & Privacy.


2. Allow the App:

In the Security & Privacy tab, under the General section, you should see a message saying that RAxML-NG was blocked from opening because it's not from an identified developer.

Click on the Allow Anyway button next to that message.


3. Open the App:
Now, try opening RAxML-NG again. You’ll still get the same warning, but this time, there should be an option to Open the application anyway.

Click Open, and it should run without further issues.

_____________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________

You'll run the RAxML-NG commands directly in the macOS Terminal.
Here's how to proceed:

Steps to Run RAxML-NG Commands:

1. Open the Terminal:

Go to Applications > Utilities > Terminal or simply search for Terminal using Spotlight (Cmd + Space).


2. Navigate to the RAxML-NG Folder:


Use the cd command to navigate to the folder where RAxML-NG was downloaded or extracted. For example:

 cd /Users/yourusername/Downloads/raxml-ng_v1.2.2_macos


Replace /Users/yourusername/Downloads/raxml-ng_v1.2.2_macos with the correct path to the folder where you have the raxml-ng binary.


3. Run the Command:


Once you're in the correct folder, run the desired command (e.g., for tree inference). For example:

 ./raxml-ng --msa /path/to/H3_Codon_Alignment.fas --model GTR+G --search1


Replace /path/to/H3_Codon_Alignment.fas with the actual path to your H3_Codon_Alignment.fas alignment file.


4. Viewing the Output:


After running the command, RAxML-NG will generate output files like RAxML_bestTree (the phylogenetic tree) and RAxML_bootstrap (the bootstrap replicates). You can view these files in the Terminal or navigate to the folder where they are saved.


Example of a Complete Command:
For instance, if your H3_Codon_Alignment.fas file is on your Desktop, and RAxML-NG is in the Downloads folder, the command might look like this:
cd ~/Downloads/raxml-ng_v1.2.2_macos
./raxml-ng --msa ~/Desktop/H3_Codon_Alignment.fas --model GTR+G --search1

Final Notes:
Make sure that you provide the full path to the input files (alignment files and tree files).


If your files are in the current directory, you can just type the filename without the full path (e.g., ./H3_Codon_Alignment.fas).

______________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________



Ensure You're in the Correct Folder:

First, check that you're in the correct directory where RAxML-NG is located. Based on your previous message, it seems you might have missed a step in navigating to the folder.


Navigate to the Folder:
Open the Terminal again, and run this command:

 cd ~/Downloads/raxml-ng_v1.2.2_macos


This should move you into the raxml-ng_v1.2.2_macos directory in your Downloads folder. Ensure the path is correct and RAxML-NG is actually located in the Downloads folder.


Check Permissions:
You encountered a "permission denied" error when trying to run RAxML-NG. You may need to give it the proper execution permissions. Run this command to do that:

 chmod +x raxml-ng


Run the Command:
Once you're in the correct folder and you've set the execute permissions, run the command again:

 ./raxml-ng --msa /path/to/H3_Codon_Alignment.fas --model GTR+G --search1


Make sure to replace /path/to/H3_Codon_Alignment.fas with the actual path to your H3_Codon_Alignment.fas file.

