
# Table of Contents

-   [examples of temporary timeouts](#xmplsftmprrytmts) [[network]]
    -   [backoff library, using it somewhere already](#bckfflbrrysngtsmwhrlrdy) 
        -   [check if kron has global timeout](#chckfkrnhsglbltmt) 
-   [network errors should be non-fatal, since they generally CAN be gracefully handled](#ntwrkrrrsshldbnnftlsncthygnrllycnbgrcfllyhndld) 
    -   [`[2019-10-19]` add to post?](#ddtpst) [[toblog]]
-   [`[2018-04-03]` Joe Duffy: the error model http://joeduffyblog.com/2016/02/07/the-error-model/](#jdffythrrrmdljdffyblgcmthrrrmdl) [[errors]]
-   [`[2019-11-22]` Error Handling Survey](#rrrhndlngsrvy) [[rust]] [[errors]]
-   [`[2018-04-05]` catching and rethrowing might be a good way of adding context](#ctchngndrthrwngmghtbgdwyfddngcntxt) [[errors]]
-   [`[2020-11-30]` Error handling is hard](#swwwfpcmpltcmblgrrrhndlngshrdrrrhndlngshrd) 
-   [Post mypy err handling on GitHub as a separate thing](#pstmypyrrhndlngngthbssprtthng) [[toblog]]
-   [hmm, so setting <span class="underline"><span class="underline">cause</span></span> doesn't really work with multiprocessing, it's lost](#hmmssttngcsdsntrllywrkwthmltprcssngtslst) [[python]] [[errors]]
-   [could probably even post to /r/programming](#cldprbblyvnpsttrprgrmmng) [[toblog]]
    -   [`[2019-10-31]` demonstrate for JS flow? https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/yield](#dmnstrtfrjsflwsdvlprmzllrdcswbjvscrptrfrncprtrsyld) 
    -   [`[2020-01-18]` eh, someone already posted?..](#hsmnlrdypstd) 





# examples of temporary timeouts      [[network]]

    requests.exceptions.ReadTimeout:
    requests.exceptions.ConnectionError:
    socket.timeout: _ssl.c:817: The handshake operation timed out
      File "/usr/lib/python3.6/socket.py", line 586, in readinto
        return self._sock.recv_into(b)
    ConnectionResetError: [Errno 104] Connection reset by peer




## backoff library, using it somewhere already

using it in vkdump  
backoff<sub>network</sub><sub>errors</sub> in kython  
I guess we could backoff indefinitely; and rely on global timeout if necessary  




### check if kron has global timeout




# network errors should be non-fatal, since they generally CAN be gracefully handled





## `[2019-10-19]` add to post?      [[toblog]]




# `[2018-04-03]` Joe Duffy: the error model <http://joeduffyblog.com/2016/02/07/the-error-model/>      [[errors]]




# `[2019-11-22]` Error Handling Survey      [[rust]] [[errors]]

<https://blog.yoshuawuyts.com/error-handling-survey>  




# `[2018-04-05]` catching and rethrowing might be a good way of adding context      [[errors]]




# `[2020-11-30]` [Error handling is hard](https://www.fpcomplete.com/blog/error-handling-is-hard/)

    Like so many other things, error handling ultimately is a trade-off. When we're writing our initial code, we don't want to think about errors. We code to the happy path. How productive would you be if you had to derail every line of code with thought processes around the myriad ways your code could fail?
    
    But then we're debugging a production issue, and we definitely want to think about errors. We curse our lazy selves for not handling an error case that obviously could have arisen. "Why did I decide to abort the process when the TCP connection failed? I should have retried! I should have logged the address I tried to connect to!"




# Post mypy err handling on GitHub as a separate thing      [[toblog]]




# hmm, so setting <span class="underline"><span class="underline">cause</span></span> doesn't really work with multiprocessing, it's lost      [[python]] [[errors]]

ugh. I guess the way to go is appending args  




# could probably even post to /r/programming      [[toblog]]





## `[2019-10-31]` demonstrate for JS flow? <https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/yield>




## `[2020-01-18]` eh, someone already posted?..

