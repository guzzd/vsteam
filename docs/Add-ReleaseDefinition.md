---
external help file: Team-Help.xml
Module Name: 
online version: 
schema: 2.0.0
---

# Add-ReleaseDefinition

## SYNOPSIS
Creates a new release defintion from a JSON file.

## SYNTAX

```
Add-ReleaseDefinition [-ProjectName] <String> [-InFile] <String>
```

## DESCRIPTION
Reads a JSON file off disk and uses that file to create a new release defintion
in the provided project.

You must call Add-TeamAccount before calling this function.

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```
Add-ReleaseDefinition -ProjectName demo -inFile release.json
```

This command reads release.json and creates a new release defintion from it
on the demo team project.

## PARAMETERS

### -InFile
Specifies the JSON file that contains the release defintion to be created.
Enter
a path and file name.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ProjectName
Specifies the team project for which this function operates.

You can tab complete from a list of available projects.

You can use Set-DefaultProject to set a default project so
you do not have to pass the ProjectName with each call.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

## INPUTS

### System.String

## OUTPUTS

## NOTES
This function has a Dynamic Parameter for ProjectName that specifies the
project for which this function gets release definitions.

You can tab complete from a list of avaiable projects.

You can use Set-DefaultProject to set a default project so you do not have
to pass the ProjectName with each call.

## RELATED LINKS
