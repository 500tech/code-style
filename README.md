# 500Tech Code Style

This repository contains all the code style settings we use at 500Tech.
 

## ESLint

There are four files for eslint:

1. .eslintrc
2. .eslintrc-angular
3. .eslintrc-react
4. .eslintrc-both

All four files share the standard rule set. The first file (without a suffix)
is a clean rule set without any plugins. The last one includes all rules both
for angular and react.

It's best to add ESLint support to WebStorm:

  1. npm i -g eslint eslint-plugin-react eslint-plugin-angular
  2. File | Default Settings | Languages & Frameworks | JavaScript | Code Quality Tools | ESLint
  3. Enable
  4. Node interpreter: /usr/local/bin/node
  5. ESLint package: /usr/local/lib/node_modules/eslint
  6. Check "Search for .eslintrc"
  7. Put .eslintrc at the root of the project

**Note:** If you use angular/react versions of the file,
          don't forget to remove the suffix in the filename.


## WebStorm Code Style

This file includes the default code style settings for WebStorm.

  1. File | Import Settings
  2. Import the file
  3. Restart WS
  4. File | Default Settings | Editor | Code Style
  5. Select "500Tech Default" scheme (on the top)
  
**Note:** You might need to apply this scheme to existing projects. 


## WebStorm Inspections

This file includes the default inspections settings for WebStorm.
This should work well together with ESLint configuration,
as the rules and the inspections are manually matched.

  1. File | Default Settings | Editor | Inspections
  2. Profile: Manage → Import
  3. Select the "500Tech Default" profile

**Note:** You might need to apply this profile to existing projects.
