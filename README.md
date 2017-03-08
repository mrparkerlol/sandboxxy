# Luvit sandbox
This sandbox is intended to be used for luvit with Discordia, but can be used without Discordia if needed. This is generally protected, but breakouts could be found still.

This is one of the many versions of my sandbox that I have written for my discord bot. It is now open-source because I don't see many lua sandboxes open sourced.

This sandbox prevents hanging of the thread by auto-terminating when execution time has exceeded 10 seconds.

To use this module, you simply need to do:
```
local sandboxxy = require('sandboxxy');
local responses = sandboxxy("print'asd'");
```

It will return a table:

`responses[1]` -> success or failure
`responses[2]` -> error ourput
`responses[3]` -> print output (if any)

You can easily do checks with these arguments if needed.

Optional checks include:
if success (`response[1]`) is false, then automatically output errors

If you find any breakouts, please don't hesitate to open an issue. I love fixing breakouts :)
