Trigger | Handler | Compatible?
--- | --- | :---: | ---
`raise` | `catch/2` | ✅
`throw` | `catch/2` | ✅
`exit` | `catch/2` | ✅
`:erlang.error` | `catch/2` | ✅
`raise` | `rescue` | ✅ 
`throw` | `rescue` | ❌ 
`exit` | `rescue` | ❌ 
`:erlang.error` | `rescue` | ✅ 
`raise` | `catch/1` | ❌ 
`throw` | `catch/1` | ✅ 
`exit` | `catch/1` | ❌ 
`:erlang.error` | `catch/1` | ❌ 


TLDR: `catch/2` will handle any kind of error.
