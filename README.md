# shelltemplate #
I noticed that I usually write the same pieces of code at the start of every
project. There's the shebang, the copyright header, the program name and the
version. This is then followed by variables that holds the path to the binaries
used in the script. After that is the sanity check to check for those binaries.
Then there is the function for printing the help screen and usage text.
So I thought it would be a good idea to keep all of this repeating code in
template. And while at it create a neat function to get all the binaries used
in the script into variables without having to manually specifiy the path by
myself. With this template I can simply just specifiy the binaries to be used
by the script and let a loop run through them and set varibles for them. This
neat little function uses the 'which' program. This means that there is only
one hardcoded binary path in the entire script. If the script fails to execute
'which' I just have to locate it manually and update a single variable. 

