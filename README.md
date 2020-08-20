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

# Experimental

## test()
\<nil\> isfile(\<void\>)

### Description
Returns void.

#### Example
```lua
print(test())
```
