
# Table of Contents

-   [related](#rltd) [[python]] [[shell]]
-   [\* pure python isn't bad for scripting](#prpythnsntbdfrscrptng) 
    -   [.](#1753_2046) 
-   [\* things I tried](#thngstrd) 
    -   [xonsh](#xnshttrlhtmlxnsh) 
    -   [plumbum](#plmbm) 
        -   [`[2015-07-18]` messing with plumbum](#mssngwthplmbm) 
    -   [http://pymotw.com/2/cmd/](#pymtwcmcmd) 
    -   [https://pypi.python.org/pypi/termcolor](#spyppythnrgpyptrmclr) 
    -   [https://pypi.python.org/pypi/sh](#spyppythnrgpypsh) 

I've had several recurring attempts to use python instead of bash in the interactive shell.  
Overall, didn't really get anywhere with it.  

The most promising was `xonsh`, a shell combining python & bash syntax. Cool idea, but I tend to forget how to use it, so never got into the habit.  

Another reasons it's not stuck to me:  

-   over the years I just got more comfortable with Bash quirks
-   now I have a better sense of when to ditch bash and just start writing a python script.  
    My personal rule of thumb is when I need something like a hashmap or array – I give up on bash that instant.

In addition, I find it nice to mix and match.  

E.g. say, you want to find out the amount of free memory  

    $ cat /proc/meminfo  | grep MemFree:
    MemFree:        23727768 kB

Right, how do we pick out the number? Normally you’d use cut, or awk:  

    $ cat /proc/meminfo  | grep MemFree: | awk '{print $2}'
    23727768

, but what if you forgot, or need something more elaborate? Well, why not use python?  

    $ cat /proc/meminfo  | grep MemFree: | python3 -c 'print(input().split()[1])'
    23727768

Not as concise as awk, but you can type it quicker than the time you’d spend googling how to use awk.  

Note that you also can use multiline input if you press enter after the opening quote, so even if you need imports etc, it doesn’t have to look horrible. Also if you have some sort of vi mode or a hotkey to edit the command in editor (`Ctrl-X Ctrl-E` in bash), it helps a lot for messing with long shell commands.  




# related       [[python]] [[shell]]




# \* pure python isn't bad for scripting





## . 

    from pprint import pprint
    from pathlib import Path
    cwd = Path('.') # make Path iterable?
    cwf.iterdir() # iterator, convert to dir
    path = cwd.join('file.png')
    path.suffix # .png
    path.stem # file
    
    from filecmp import cmp




# \* things I tried





## [xonsh](http://xon.sh/tutorial.html) 

-   importing local modules  
    
        import sys
        sys.path.insert(0, '')
-   no way of using source as in bash?
-   DIR = os.path.dirname(os.path.abspath(sys.argv[0])) (TODO move it to python preamble?)




## plumbum 

<http://plumbum.readthedocs.io/en/latest/>  




### `[2015-07-18]` messing with plumbum

    from plumbum import local, ProcessExecutionError
    from plumbum.commands.modifiers import RETCODE, BG
    
    hg  = local['hg']
    git = local['git']
    
    if hg['status'][path] & RETCODE == 0:
        with local.cwd(local.cwd / path):
          pass
          # execute the local command
    
    ret, out, err = git['config', 'branch.master.remote'].run(retcode=0) # expected retcode




## <http://pymotw.com/2/cmd/> 




## <https://pypi.python.org/pypi/termcolor> 




## <https://pypi.python.org/pypi/sh> 

