= What is this
Peercast for Linux + VP patch + fixed compile bug
  
= Compile
 $ cd ./ui/linux/
 $ make

= Run
 # run background
 $ cd ./ui/linux/
 $ vi peercast.ini # edit
 $ ./peercast &
 $ disown

 # download stream
 $ curl "http://localhost:7144/pls/90FB65E262ED3BAC00F02E363777****?tip=xx.yy.zzz.pp:7144"
<ASX Version="3.0">
<TITLE>**ch</TITLE>
<MOREINFO HREF = "http://example.com/path/to/channel" />
<ENTRY>
<TITLE>**ch</TITLE>
<MOREINFO HREF = "http://example.com/path/to/channel" />
<REF href = "mms://127.0.0.1:7144/stream/90FB65E262ED3BAC00F02E363777****.wmv" />
</ENTRY>
</ASX>

 $ mplayer -dumpstream mms://127.0.0.1:7144/stream/90FB65E262ED3BAC00F02E363777****.wmv -dumpfile /path/to/output.wmv

