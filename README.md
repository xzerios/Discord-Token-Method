# How To Obtain Your Discord Token
This is a way to obtain your Discord token almost immediately! That means no more hassle with the application layer!

- Open your browser's console window. This can be reached through f12 and then clicking "Console"
- Open Discord
- Paste this into the console:

*Simple Version*
```
(webpackChunkdiscord_app.push([[''],{},e=>{m=[];for(let c in e.c)m.push(e.c[c])}]),m).find(m=>m?.exports?.default?.getToken!==void 0).exports.default.getToken()
```
*Beautified*
```
(
    webpackChunkdiscord_app.push(
        [
            [''],
            {},
            e => {
                m=[];
                for(let c in e.c)
                    m.push(e.c[c])
            }
        ]
    ),
    m
).find(
    m => m?.exports?.default?.getToken !== void 0
).exports.default.getToken()
```
- Your token then gets printed to console
- Or use this code which automatically copies it to clipboard:
```
window.webpackChunkdiscord_app.push([[Math.random()], {}, (req) => {for (const m of Object.keys(req.c).map((x) => req.c[x].exports).filter((x) => x)) {if (m.default && m.default.getToken !== undefined) {return copy(m.default.getToken())}if (m.getToken !== undefined) {return copy(m.getToken())}}}]); console.log("%cIt worked!", "font-size: 50px"); console.log(`%cYou now have your token in the clipboard!`, "font-size: 16px")
```
