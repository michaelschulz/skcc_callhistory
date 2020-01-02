# SKCC Call History 

This is the current (1/1/2020) SKCC member list converted for use 
in N1MM as call history file which allows auto fill of information.

Conversion can be done with simple one liner in Bash:

cat skcclist.txt | sed s/" "/""/g |sed s/'|'/' '/g | awk '{ print $2"," $3","$5","$1}' > skcc_call_history.txt  
