# Reproducing this issue

1. Clone this repo
2. `npm i` (I am using node v11.15.0)
3. Open test.ts with coc.nvim enabled
4. `:CocInstall coc-eslint`

You should see the error message when the language server starts:

```
[coc.nvim] error: UnhandledRejection: Range#create called with invalid arguments[null, -1, null, 0]
Error: Range#create called with invalid arguments[null, -1, null, 0]
    at Object.create (/Users/Mike/bin/dotfiles/vim/plugged/coc.nvim/build/index.js:17773:19)
    at DiagnosticBuffer.fixRange (/Users/Mike/bin/dotfiles/vim/plugged/coc.nvim/build/index.js:51766:55)
    at diagnostics.forEach.o (/Users/Mike/bin/dotfiles/vim/plugged/coc.nvim/build/index.js:51577:36)
    at Array.forEach (<anonymous>)
    at Timeout.setTimeout [as _onTimeout] (/Users/Mike/bin/dotfiles/vim/plugged/coc.nvim/build/index.js:51576:29)
    at ontimeout (timers.js:436:11)
    at tryOnTimeout (timers.js:300:5)
    at listOnTimeout (timers.js:263:5)
    at Timer.processTimers (timers.js:223:10)
[coc.nvim] error: UnhandledRejection: Range#create called with invalid arguments[null, -1, null, 0]
Error: Range#create called with invalid arguments[null, -1, null, 0]
    at Object.create (/Users/Mike/bin/dotfiles/vim/plugged/coc.nvim/build/index.js:17773:19)
    at DiagnosticBuffer.fixRange (/Users/Mike/bin/dotfiles/vim/plugged/coc.nvim/build/index.js:51766:55)
    at diagnostics.forEach.o (/Users/Mike/bin/dotfiles/vim/plugged/coc.nvim/build/index.js:51577:36)
    at Array.forEach (<anonymous>)
    at Timeout.setTimeout [as _onTimeout] (/Users/Mike/bin/dotfiles/vim/plugged/coc.nvim/build/index.js:51576:29)
    at ontimeout (timers.js:436:11)
    at tryOnTimeout (timers.js:300:5)
    at listOnTimeout (timers.js:263:5)
    at Timer.processTimers (timers.js:223:10)
```
