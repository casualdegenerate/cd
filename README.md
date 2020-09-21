# cd
:)

# File

## ISFILE
\<boolean\> isfile(\<string\> pathToFile)

### Description
Will return a true or false statement on if the file exist or not.

#### Example
```lua
if isfile("cd/Chat.txt") then
	print("File Exist")
else
	print("File Does Not Exist","Creating File!")
	writefile("cd/Chat.txt","")
end
```

## ISFOLDER
\<boolean\> isfolder(\<string\> pathToDirectory)

### Description
Will return a true or false statement on if the folder exist or not. (Note: The way I wrote isfolder in the script makes it a little bit wack, but I will update it to be better, I promise :))

#### Example
```lua
if isfolder("cd") then
	print("Folder Exist")
else
	print("Folder Does Not Exist")
end
```

# In-Game Use

## RCHAT
\<void\> rchat(\<string\>)

### Description
Will run any game:GetService("Players").LocalPlayer.Chatted connections without saying anything in chat

#### Example
```lua
rchat(":respawn me")
```

## FCHAT
\<void\> fchat(\<string\>)

### Description
Will type in chat without hitting any game:GetService("Players").LocalPlayer.Chatted connections

#### Example
```lua
fchat("Hi.")
```

## TCHAT
\<void\> tchat(\<string\>)

### Description
Will use both rchat and fchat so if you want to use both the real chat and fake chat to simulate talking in game normally

#### Example
```lua
tchat("Hello.") 
```

## OUTFIT
\<void\> outfit(\<string\> Directory)

### Description
Will give the client an outfit that has information writen in file in the directory ("cd/Outfits/$id$.cd")

#### Example
```lua
Outfit("550673488") 
```
Must have the file itself made first. (You can join my server and ask the bot I made for the module made for you. 7F4uz8h
```lua
local outfit = {
	["Hat"] = {
		"5099663350",
		"5355196085",
		"5355304172",
		"5372331709",
	},
	["Shirt"] = "2746996347",
	["Pants"] = "5194178265",
	["Face"] = "0"
}
return outfit
```

# String

## STRINGTOBYTE
\<string\> stringtobyte(\<string\>)

### Description
Will turn a bunch of characters in a string like "Test" to "\84\101\115\116" so you don't need to make a function yourself to make a large string into a byte if needed.

#### Example
```lua
print(stringtobyte("hhhh, imagine really using this like, lmao?")
```

# Data

## ~~ISFRIENDS~~ Depricated, Use (https://developer.roblox.com/en-us/api-reference/function/Player/IsFriendsWith)
~~\<boolean\> isfriends(\<number\>,\<number2\>)~~

### ~~Description~~
~~Will return true if the too player IDs are friends with each other. Used to collect mass data on players for the fun of it or to use it as esp to tell straight away if two players are friends and are teaming or something along those lines if that is what you intead for it.~~

#### ~~Example~~
~~game:GetService("Players").PlayerAdded:connect(function(plr)~~
	~~for _,v in pairs(game:GetService("Players"):GetPlayers()) do wait(1) --Don't spam too many request.~~
		~~if isfriends(v.UserId,plr.UserId) then~~
			~~print(plr.Name,"Is friends with",v.Name)~~
		~~end~~
	~~end~~
~~end)~~
~~Will work aslong as you don't HTTP429. Okay?~~

# Experimental

## IS_CD_CALLER
\<boolean\> is_cd_caller(\<void\>)

### Description
Returns true if you are using this API. It's a way to check if you have the API and working!

#### Example
```lua
if is_cd_caller then
	print("Found API!")
else
	print("Did Not Find API?","Call 586141923048161291 for help.")
end
```

# Undocumented
countfriends

# h
msg me if you have any useful functions that would just make life easier to me so I can add them
