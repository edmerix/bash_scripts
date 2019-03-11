# bash_scripts
A very minimal selection of bash scripts I use here and there.

## Files:
### nsxdetails

Quick 'n' easy reading of the header of .NSx files of neural data from Blackrock recordings (NPMK is slooow)

Especially useful for finding data when sync'd NSPs were used - the output includes:
  
- True recording start and finish times (in local time, not UTC)

- Number of data segments (syncing NSPs causes "paused" files, file-turnover errors cause many segments)

- Duration of each segment

- Total duration of data in the file

- Sampling frequency and number of data samples

- Number of channels



### nsxtimes

Run in any directory to list the actual (local) start times of all NSx files in that directory

Pass in an optional parameter to set which type of NSx file (defaults to NS3)


### nytcli

A (colorful) CLI for browsing the most recent headlines from the New York Times.

Need to get/set your own [API key](https://developer.nytimes.com) on line 17 for this to function.

Flags:

* -s: _set a specific section to read headlines from (defaults to all)_

* -l: _limit the number of headlines returned (defaults to 15)_

* -h: _show the help, and returns a list of allowable "sections"_

Once running, enter the ID number of an article to read its abstract, or enter one of the following "commands":

* h: _show the **h**elp_

* l: _re-show the loaded headlines (**l**ist)_

* r: _open the most recently selected article in the default browser (**r**ead)_

* q: _**q**uit_
    
