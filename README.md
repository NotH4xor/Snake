# Script
```
local scripts = {
    'https://raw.githubusercontent.com/NotH4xor/Snake/main/X_Teleport',
    'https://raw.githubusercontent.com/NotH4xor/Snake/main/R_Key',
    'https://raw.githubusercontent.com/NotH4xor/Snake/main/F_Key',
}
for _, url in ipairs(scripts) do
    local thread = coroutine.create(function()
        loadstring(game:HttpGet(url, true))()
    end)
    coroutine.resume(thread)
end
table.insert(scripts, "new_script_url")
```
