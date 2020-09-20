### Remote
 The "remote" command helps you to manage connections to remote repositories.
 It allows you to show which remotes are currently connected, but also to add new connections or remove existing ones.
 ####-v
 Shows URLs of remote repositories when listing your current remote connections. 
 By default, listing remote repositories only shows you their shortnames (e.g. "origin"). 
 Using the "-v" option, you will also see the remote's URLs in listings.
 Example: git remote -v
 ####add <shortname> <url>
 Creates a new connection to a remote repository.
 The "shortname" you provide can later be used instead of the URL when referencing the remote. 
 A typical default shortname is "origin": this is used for the remote which your local repository was cloned from.
 Example: git remote add test test@github.com/test/example.git
 ####remove <name>
 Disconnects the remote from the local repository. 
 Note that this will have no effect on the actual remote repository (i.e. the repository itself is not removed / deleted / etc.).
 Example: git remove test


