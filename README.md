# kailua_setup
Files required for initial setup of Kailua for TW:WH2. If this needs updating, please find me on the C&amp;C Modding Den.

--------

I don't know GitHub markdown, nor do I care enough right now to figure it out. Just writing out this tutorial before I go to bed.

So! All we gotta do. Repeat after me.

STEP ONE: Download Visual Studio Code.

STEP TWO: Download SourceTree, or another GitHub frontend program if you prefer.

STEP THREE: In Visual Studio Code, select "Extensions" in the side bar on the left (by default). Search "Kailua", and download it.

STEP FOUR: Make a GitHub account if one is not already made, and then create a public or private - your choice! - repository.

STEP FIVE: In the new GitHub Repo page, select "Clone or Download", and copy the link.

STEP SIX: Open up SourceTree, select File -> Clone/New... -> Paste your repo code in Source Path / URL.
-- Destination Path, make it a sensical location on your Computer where you'd like to save your local script files.
-- Name, make it equally sensical.

STEP SEVEN: Download the .vscode and example folders from this here repo. You can just download the .zip, or whatev.

STEP EIGHT: Add those folders exactly as they are to your new folder! You will probably want to remove /example eventually, but for early purposes, keep it in. It's not hurting anybody.

STEP NINE: Open up VSCode, select File -> Add Folder to Workspace... -> browse to your Destination Path.

STEP TEN: I like working in Workspaces. They make it really easy to go between one project to the next. So, I recommend saving the workspace. Select File -> Save Workspace As... -> save it somewhere sensical.

STEP ELEVEN: Go back to SourceTree. On "Unstaged files" press "Stage All". In the top left press "Commit". A prompt will appear at the bottom asking you to type in a quick description of the changes. I put in "Initial Commit" for my first one, and then I keep a small description for changes afterwards. After that, press "Commit", on now the bottom right.

And that's it! You now have your own GitHub Repo, VSCode set up, a GitHub frontend program, and a VSCode Extension that will read many TW:WH2 functions, types, and the like.

To get Kailua enabled on your scripts, add them to the workspace, NOT in the .vscode folder. They can be in a subfolder to the main folder, like "example.lua" is, or in the main folder itself at the same level as .vscode. After the file is added, go to .vscode/entry.lua, and type in
require("file")
or, if in a folder
require("folder/file")
or, if in many folders
require("folder/folder2/file")
and so on. You do NOT need the ".lua" specified in that command, it will only look for .lua files. 

Right now, the "example.lua" file is completely blank, I will be working on that later. I will also be explaining Kailua directives, to solve some errors/warnings you might be having early on. But for now, I want to go to bed, enjoy.
