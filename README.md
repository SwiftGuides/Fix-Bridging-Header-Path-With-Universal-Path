# Fix-Bridging-Header-Path-With-Universal-Path
This guide will will Bridging-Header.h Path issue and give it a universal path so It can Adapt Path Automatically


Source :- https://stackoverflow.com/a/28551452/10422074

1. This requires the following value for the setting: Targets > [Your App Target] > Build Settings > Swift Compiler - Code Generation > Objective-C Bridging Header

```
$(SRCROOT)/$(PROJECT_NAME)/$(PROJECT_NAME)-Bridging-Header.h 

```

#### Note :- that if your project is a swift module (framework) then, as pointed out in the comments, you might prefer 

### (Highly Recommended)

```
$(SRCROOT)/$(PROJECT_NAME)/$(SWIFT_MODULE_NAME)-Bridging-Header.h

```
