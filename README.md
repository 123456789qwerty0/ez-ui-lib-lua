# ez-ui-lib-lua
usage:
Window(<string> title)
   Toggle(<string> text, <function> callback)
   Slider(<string> text, <table> options {max, default}, <function> callback)
   ______________________________________________________________________
   example:
   local lib = loadstring(game:HttpGet('https://raw.githubusercontent.com/123456789qwerty0/ez-ui-lib-lua/main/main.lua'))()
local window = lib:Window('title here')

window:Toggle('toggle', function(enabled)
     print(enabled)
end)

window:Slider('slider', {
     max = 80,
     def = 20
}, function(value)
     print(value)
end)
