# lib_AppShorter
Convertigo Application Shorter.
This Library enables shortcuts to applications by using simple URLs of type http(s)://&lt;server&gt;:&lt;Port&gt;/&lt;shortcut&gt;

## Installation
Deploy this Library in any existing Convertigo Server Instance..

## Usage
The library provides several sequences you can run from the test platform :

* Connect to https://&lt;yourserver&gt;:&lt;Port&gt;
* Authenticate to the test platform using admin user & password (Upper right)
* Open the Sequence Section
* Run one of the following sequences.

| Sequence | Usage |
|----------|-------|
| list  | List all shortcuts defined |
| set   | set a shortcut to an app |
| unset | delete a shortcut to an app |

  
### __set__ variables
* __project__ : the Convertigo project name holding the target application. This is Case sensitive
* __name__    : the shortcut name. If not provided the project name will be used automatically.
  
### __unset__ variables
* __name__    : the shortcut name
  
  
