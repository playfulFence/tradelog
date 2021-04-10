# tradelog
Bash script created to conviniently and productively display and organize your log-files from te stock exchange


Usage: tradelog [-h|--help]
        tradelog [FILTER...] [COMMAND] [LOG...]
      
        ---------------------------------------DETAILED DESCRIPTION------------------------------------
          COMMAND can be ONE of:
        |-----------------------------------------------------------------------------------------|
        |• list-tick -- a list of occurring stock exchange symbols, so-called \"tickers\".        | 
        |-----------------------------------------------------------------------------------------|
        |• profit -- statement of total profit from closed positions.                             |
        |-----------------------------------------------------------------------------------------|
        |• pos -- list of values of currently held positions sorted in descending order by value. | 
        |-----------------------------------------------------------------------------------------|
        |• last-price -- list of the last known price for each ticker.                            | 
        |-----------------------------------------------------------------------------------------|
        |• hist-ord -- shows the histogram of the number of transactions according to the ticker. | 
        |-----------------------------------------------------------------------------------------|
        |• graph-pos -- shows the graph of values of held positions according to the ticker.      | 
        |_________________________________________________________________________________________|

              The FILTER can be a COMBINATION of:
        |---------------------------------------------------------------------------------------------|
        |• -a DATETIME -- after: only records AFTER this date (without this date) are considered.     |   
        |                DATETIME is in the format YYYY-MM-DD HH:MM:SS.                               |
        |---------------------------------------------------------------------------------------------|
        |• -b DATETIME -- before: only records BEFORE this date (without this date) are considered.   |
        |               DATETIME is in the format YYYY-MM-DD HH:MM:SS.                                |
        |---------------------------------------------------------------------------------------------|
        |• -t TICKER -- only records corresponding to the given ticker are considered.                |
        |             With multiple occurrences of the switch, the set of all listed ticker is taken. |
        |---------------------------------------------------------------------------------------------|
        |• -w WIDTH -- sets the width of the GRAPH listing, the length of the longest line to WIDTH.. |
        |              Thus, WIDTH must be a positive integer                                         |
        |             Multiple occurrences of the switch is a faulty start.                           | 
        |---------------------------------------------------------------------------------------------|
        |• -h and -help -- print help with a brief description of each command and switch.            |
        |____________________________________________________________________by_playfulFence__________|
