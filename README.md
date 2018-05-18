# cloud9restore
This script can restore deleted files in a Cloud9 workspace. This only works for files that you edited in the cloud9 editor.

It mines the versioning database and looks for files that are in this database but not in the file system.

# installation:
	wget https://rawgithub.com/simonpauw/cloud9restore/master/restore
	chmod a+x restore
	mv ./restore ~/bin/restore

# example usage:
	$ restore
	$ 0:    ~/workspace/pset1/somefile-I-deleted.c
	$ 1:    ~/workspace/pset1/some-orhter-file-I-deleted.c
	$ Enter file# to restore (or anything else to quit): 0
	$ Restored ~/workspace/pset1/somefile-I-deleted.c