# Sage2Kodi
FileRenamer for SageTV for proper Kodi naming
This project is still in Beta please perform test renaming before trusting.
Here is a brief description of the settings. To access wihout editing xml pass "/settings" to the cmd prompt.

"SageServerHttp"

This is the http or https address of your BMT webserver (sagetv server).

"DeleteAfterCopy"

Please use with CAUTION! This is irreversible. It compares file sizes before deleting original--*Plan to add hash checks down the line for further guarantee 
the file copied correctly. USE AT OWN RISK

"UserName"

UserName for BMT web interface

"Password"

Password for BMT web interface

"SourceLocation"

Which directories do you want to rename "From" (you can use network or local pathnames). Can add multiples with <string> tag

"NewLocation"

Location you want the renamed files moved to. (again local or network paths)

"InclArticleFiles"

Choose to include article files with move. Must be named as original and in same location. 

"Extensions"

Extensions of video files you want renamed (ie mkv etc) can have multiple with <string> tag

"TvSubFolder"

Tv sub folder of new location . IE if new location is c:\movieskodi this is the subfolder created under that for TV files

"MovieSubFolder"

Same as tv subfolder except for movies

NOTE: Movies and TV are identified the same as in BMT

"RunTestOnly"

This is a test run and uses the small test.mpg file in the source to run a quick test rename/copy to verify your settings quickly.

"IgnoreDuplicateFiles"

If duplicates are found this option chooses wether to ignore or still copy

"ScrubStartingArticlestoEnd"

Move the, a , an to the end of title (recommended for Kodi Import)

"MovieFileRenamParams" & "MovieFolderRenamParams" & "TVFileRenamParams" & "TVFolderRenamParams"

How you want you  files and folders renamed  ":" equals space or you can space. Any value from the sage metadata can be put here anything pulled from sage needs to 
be in enclosed in "{}". The ones in default are custom but the @MediaFilaID is an example of pulling straight from SageX Provided xml.

"DeleteLowerResolutionOnReplacement"

These will use resolution priority to delete a lower resolution file from the existing renaming directoy. (must have resoltuion in the file name and must be same format as same in 
naming scheme)

"UseResolutionNames"

Use resolution names inplace of 1080i etc

"ResolutionOrder"

Your preference resolution order from highest to lowest 

"ResolutionNames"

Names used to replace resolutions if "UseResolutionNames" is set to true. Must be in same order and have same amount as "ResolutionOrder" or it will fail.

"ArticleExtensions"

extensions of articles to move and rename if set to true (ie jpeg, properties etc)

"DuplicateAdder"

Adder to add to end of duplicate files if ignore duplicates is set to true and duplicates are found.

"MoveDuplicatesToSpecialFolder"

This will move duplicates to special folders to help locate them if wanted

"DuplicatesFolder"

Name of duplicates folder.

"RenameMultiSegments"

This is for multi segments (ie sage stopped and restarted recording for some reason). Still not fully tested



