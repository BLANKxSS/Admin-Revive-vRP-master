Hello,

I made simple code for vrp for admin can revive with server id 

>how install 
go to vrp/modules/admin.lua and add the code on anywhere 

http://prntscr.com/l9ge4w

http://prntscr.com/l9gev4

> how to use 
go to Admin then you will see Admin revive just put server id for the player 

not tested on public servers , use as own your risk

you can edit to use user id instead server id

-- Made by Sul6an for vRP freamwork
-- install on vrp/modules/admin.lua 
-- not tested on public servers , use as own your risk



-----------------------------------------------------------------------------------
		 if vRP.hasPermission(user_id,"player.adminrevive") then
          menu["Admin Revive"] = {ch_revive_stn}
        end
	
	
local function ch_revive_stn(player,choice) -- Admin Revive 
  local user_id = vRP.getUserIdentity(user_id)
  if user_id ~= nil then
    vRP.prompt(player,"Revive:","",function(player,user_id) 
	  	vRPclient.varyHealth(user_id, {100})
    end)
  end
end
		

sorry for bad lang.
