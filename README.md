# cd
:)

# File

## isfile()
\<Boolean\> isfile(\<string\> pathToFile)

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

## isfolder()
\<Boolean\> isfolder(\<string\> pathToDirectory)

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

# Experimental

## is_cd_caller()
\<Boolean\> is_cd_caller(\<void\>)

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

## test()
\<nil\> isfile(\<void\>)

### Description
Returns void.

#### Example
```lua
print(test())
```
