# Repo watch
This small script checks svn and git repositories for changes.

## Usage
First of all fill the files `repos-git.txt` and `repos-svn.txt` with URLs of repositories, one URL per line.

Then run the [watch](./watch)-script once to fetch the current state of each repository. The current state is written to a file called `versions.txt`.

At every consecutive run of the script, the new state of each repository will be fetched and the changes are the printed to the screen as the diff of the files `versions.txt` and `versions-old.txt`. `versions.txt` always holds the state from the last run of the script, `version-old.txt` holds the state of the run before.
