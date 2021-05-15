
# Table of Contents

-   [shell programming](#shllprgrmmng) [[bash]]
    -   [`[2017-12-25]` boolean return value](#blnrtrnvl) 
    -   [`[2017-12-26]` multi-line string varible](#mltlnstrngvrbl) 
    -   [`[2017-12-30]` iterate over array](#trtvrrry) 
    -   [assert variable is defined {double square brackets -v} operator](#ssrtvrblsdfnddblsqrbrcktsvprtr) [[habit]]
    -   [`[2018-04-26]` get current script directory](#gtcrrntscrptdrctry) 
    -   [avoid passing flags in shebang (e.g. `#!/bin/bash -eu`)](#vdpssngflgsnshbnggbnbsh) [[habit]]
-   [interactive tricks & tips](#ntrctvtrckstps) [[shell]]
    -   [`[2015-07-23]` `diff <(ls dir1) <(ls dir2)`](#dfflsdrlsdr) 
    -   [use sigquit {Ctrl-\\} to kill processes that are really stuck (when Ctrl-C isn't working)](#ssgqtctrltkllprcsssthtrrllystckwhnctrlcsntwrkng) [[habit]]
    -   [exec command on each file `find . -exec some command {} \;`](#xccmmndnchflfndxcsmcmmnd) [[drill]]
    -   [exec command in parallel `find /path -iname '*.pdf' -print0 | xargs -0 -n1 -i -P8 bash -c "echo 'Processing {}' && command '{}'"`](#xccmmndnprlllfndpthnmpdfptxrgsnpbshcchprcssngcmmnd) [[drill]]
    -   [`[2018-05-08]` `ps aufx` to list all processes](#psfxtlstllprcsss) 
    -   [tree -pufi for file tree with permissions](#trpffrfltrwthprmssns) [[habit]]
    -   [pretty print json `cat file.json | python -mjson.tool`](#prttyprntjsnctfljsnpythnmjsntl) [[json]]
    -   [detect if library is installed `ldconfig -p | grep libjpeg` or `gcc -ljpeg`](#dtctflbrrysnstlldldcnfgpgrplbjpgrgccljpg) 
    -   [`[2015-07-23]` merging pdfs](#mrgngpdfs) 
    -   [{ln -i} for interactive symlink (prompts for removal)](#lnfrntrctvsymlnkprmptsfrrmvl) [[habit]]
-   [use whiptail for ncurses dialogs](#swhptlfrncrssdlgs) [[tui]] [[habit]]
-   [`[2021-01-06]` Where is the bash feature to open a command in $EDITOR documented? - Unix & Linux Stack Exchange](#snxstckxchngcmqstnswhrsthdndtrdcmntdnxlnxstckxchng) [[bash]] [[habit]]

Bash & shell programming  




# shell programming      [[bash]]





## `[2017-12-25]` boolean return value

    function whatever {
     if (x)
      then
          true
      else
          false
      fi
    }
    if whatever
    then ...




## `[2017-12-26]` multi-line string varible

    MULTILINE=$(cat <<-END
    here
    goes
    multi
    line
    END
    )




## `[2017-12-30]` iterate over array

    EXTRA_STOWS=("home-arbtt" "home-emacs" "home-anacron")
    for s in "${EXTRA_STOWS[@]}"




## assert variable is defined {double square brackets -v} operator      [[habit]]




## `[2018-04-26]` get current script directory

    DIR=$(dirname "$(readlink -f "$0")")

(might not work on mac)  




## avoid passing flags in shebang (e.g. `#!/bin/bash -eu`)      [[habit]]

e.g. if you specify other flags in terminal, they would override everything  
instead, better to use `if [[ $0 == "$BASH_SOURCE" ]]; then set -eux; fi`  




# interactive tricks & tips      [[shell]]

priorities roughly indicate how useful I find each command  




## `[2015-07-23]` `diff <(ls dir1) <(ls dir2)`




## use sigquit {Ctrl-\\} to kill processes that are really stuck (when Ctrl-C isn't working)      [[habit]]




## exec command on each file `find . -exec some command {} \;`      [[drill]]




## exec command in parallel `find /path -iname '*.pdf' -print0 | xargs -0 -n1 -i -P8 bash -c "echo 'Processing {}' && command '{}'"`      [[drill]]




## `[2018-05-08]` `ps aufx` to list all processes




## tree -pufi for file tree with permissions      [[habit]]




## pretty print json `cat file.json | python -mjson.tool`      [[json]]




## detect if library is installed `ldconfig -p | grep libjpeg` or `gcc -ljpeg`




## `[2015-07-23]` merging pdfs

    pdftk out.pdf j1-process.pdf j1-process-2.pdf j1-process-3.pdf cat output merged.pdf
    pdftk full-pdf.pdf cat 1 1 1 2  3 4 12-15 output outfile_p12-15.pdf




## {ln -i} for interactive symlink (prompts for removal)      [[habit]]




# use whiptail for ncurses dialogs      [[tui]] [[habit]]




# `[2021-01-06]` [Where is the bash feature to open a command in $EDITOR documented? - Unix & Linux Stack Exchange](https://unix.stackexchange.com/questions/85391/where-is-the-bash-feature-to-open-a-command-in-editor-documented)      [[bash]] [[habit]]

    edit-and-execute-command (C-xC-e)

