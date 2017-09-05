# wsj
Simple Bash script to download the Wall Street Journal for free (Mac Only). I built this as a gift for my Dad after he alerted me one can read the WSJ every day for free by just editing the URL with the exact date (YYYYMMDD format), section (A, B, C, D, or M), and page number (001 - 020) that you want to view. 


For example, if you want to view page A1 of the November 9th, 2016 WSJ, you can do so by viewing the URL: http://online.wsj.com/public/resources/documents/print/WSJ_-A001-20161109.pdf . I wonder if that was an important news day... 


This repo contains a single Bash script (untested on other *nix platforms for compatibility just yet) which will download an entire day's edition of the Wall Street Journal. 

When the program runs, it prompts the user for input on what day's paper he/she would like to download. Appropriate inputs include "today", "yesterday", or an 8 character date in format YYYYMMDD (such as 20161109). 

The program then determines what day of the week the download has been requested for (to figure out which sections it needs to look for - check the script comments for an explanation of this). For example, if the user enters a date in the past, the program will figure out what day of the week the requested date was before downloading. Please note the WSJ does not publish on Sundays, so any date that is recognized as a Sunday causes the program to exit without attempting any download. 

Once the script completes downloading all possible pages for the requested day's paper, it will automatically open all of the downloaded PDFs in the user's default PDF viewer (this will be Preview for a majority of Mac users I presume).


To run this:

	1. Place the "getPaper" file on your Mac Desktop (easiest) or anywhere else convenient for you.
 
	2. To give the script permission to execute, you might need to run $ chmod 755 <yourPath>/getPaper.

	3. Double-click the executable file (or run it in terminal, no parameters needed) and follow the instructions.

Enjoy!
- Tom

www.tomd.tech 



