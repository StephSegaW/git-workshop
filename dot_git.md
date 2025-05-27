## What is .git?
The .git folder stores your Git Repo'd full history. It is typically hidden because of the . to prevent accidental changes. 

### Command bash 

    ls -a .git

### In terminal output

    steph@DESKTOP-BAUP435 MINGW64 /c/Repos/ReDISchoolGitHub/GitHubWorkshop/git-workshop (master)
    $ ls -a .git
    ./  ../  config  description  FETCH_HEAD  HEAD  hooks/  index  info/  logs/  objects/  packed-refs  refs/

    steph@DESKTOP-BAUP435 MINGW64 /c/Repos/ReDISchoolGitHub/GitHubWorkshop/git-workshop (master)
    $


Never delete or change it, unless you know what you are doing. This may break your Repo! 

### DIAGRAM FOLDER STRUCTURE
```
.git/
├── HEAD               ← Pointer to your current branch (like main or dev)
├── config             ← Settings like user name, remote repo URL, etc.
├── description        ← Used by some Git tools (often ignored)
├── index              ← The staging area (snapshot of changes to commit)
├── hooks/             ← Scripts that run at certain Git events (optional)
├── info/              ← Exclude rules or other local-only settings
├── logs/
│   └── HEAD           ← History of branch movements
├── objects/           ← Actual content of your files and commits
│   ├── [hash folders] ← Commit, tree, and blob objects (compressed)
├── refs/
│   ├── heads/         ← Local branches (e.g., main, dev, feature-x)
│   ├── tags/          ← Tags for releases
│   └── remotes/       ← Tracking branches from remotes (like origin)


