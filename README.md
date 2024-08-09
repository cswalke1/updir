# updir
A tool to navigate linux directories up-the-chain from the command line

# usage

Put the .updir.sh file in your home directory 
and add to your .bashrc file:
```
. .updir.sh
#or
source .updir.sh
```

# help
```
    updir - go up parent directories
usage:
    updir [-r] <#>                will go up # directories
    updir [-r] <search>           will go up till it finds <search>, can be just the beginning of the directory name
    updir [-r] <search> <#>       same as 'updir <search>' except if there are directories further up the chain that match will choose <#> of matches further up
    updir [-r] -s <search>        the -s flag will force search to be a search term, even if it is a number (directories can be named by a number after all)
    updir [-r] -s <search> <#>
    -r option                     will print the folder and not change directory to it
    updir -h                      display this usage
    updir -e                      display examples

    tab-completion works with this command

-*NOTICE*-  clears the following environment variables: tmp_re, tmp_amount, tmp_search, tmp_cur, tmp_dirs, OLD_IFS     usually no problem at all , Will make these local in a future version.  Sorry not that saavy with shell scripting atm.
```
