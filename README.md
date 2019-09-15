# Tover's HUD
By Tover , Tover's Services

Do you want more of these high-quality scripts ? Feel free to join my discord https://discord.me/tover

#What to do ?
1) Be sure to install esx_status and esx_basicneeds
2) In esx_basicneeds replace line 42 til 52 with
```lua
TriggerEvent('esx_status:registerStatus', 'hunger', 1000000, '#CFAD0F', function(status)
		return false
	end, function(status)
		status.remove(100)
	end)

	TriggerEvent('esx_status:registerStatus', 'thirst', 1000000, '#0C98F1', function(status)
		return false
	end, function(status)
		status.remove(75)
	end)
```

3) Or just simply replace `return true` to `return false` on line 43 and line 49
[Optional]
4) Go to es_extended/config.lua and set `Config.EnableHud` to false


Enjoy the HUD !
