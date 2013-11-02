SampleWebAPI
=========

This is a vanilla `File -> New Project -> MVC Internet Website` project with a goal of demonstrating how you might use [ToTypeScriptD](http://github.com/ToTypeScriptD/ToTypeScriptD) to generate `TypeScript` type definition (`.d.ts`) files automatically from your `.Net` assembly(s).

# Install [ToTypeScriptD](http://github.com/ToTypeScriptD/ToTypeScriptD) with [Chocolatey](http://chocolatey.org)

    cinst ToTypeScriptD

### Get the type definitions out of your MVC project

    ToTypeScriptD SampleWebAPI\bin\SampleWebAPI.dll

### Save the output to a file

    ToTypeScriptD SampleWebAPI\bin\SampleWebAPI.dll > SampleWebAPITypeDefinitions.d.ts

### Only get types in a specific namespace

    ToTypeScriptD SampleWebAPI\bin\SampleWebAPI.dll --regexFilter "SampleWebAPI.Controllers"
