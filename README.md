# SKCC Call History 

This is the current (1/1/2020) SKCC member list converted for use 
in N1MM as call history file which allows auto fill of information.

Conversion can be done with a simple (and crude) one liner in Bash:
 
 tail -n +2 skcclist.txt | sed s/" "/""/g |sed s/'|'/' '/g | sed -e '1i\!!Order!!,Call,Name,Exch1,Misc' |awk '{ print $2"," $3","$5","$1}' |sed s/,,,/"" /g > skcc_call_history.txt