# lib_AppShorter
Convertigo Application URL Shortener.
This Library enables shortcuts to applications by using simple URLs of type http(s)://&lt;server&gt;:&lt;port&gt;/&lt;shortcut&gt;

## Installation
Deploy this Library in any existing Convertigo Server Instance or Studio using one of the ***Convertigo Project URL***:
* From ZIP: `lib_AppShorter=https://github.com/convertigo/c8oprj-lib-app-shorter/archive/refs/heads/7.9.0.zip`
* Clone (https): `lib_AppShorter=https://github.com/convertigo/c8oprj-lib-app-shorter.git:branch=7.9.0` 
* Clone (ssh): `lib_AppShorter=git@github.com:convertigo/c8oprj-lib-app-shorter.git:branch=7.9.0`

## Usage
The library provides several sequences you can run from the test platform :

* Connect to https://&lt;yourserver&gt;:&lt;port&gt;
* Authenticate to the test platform using admin user & password (Upper right)
* Open the Sequence Section
* Run one of the following sequences.

| Sequence | Usage |
|----------|-------|
| list  | List all shortcuts defined |
| set   | set a shortcut to an app |
| custom| set a shortcut to a custom Convertigo URL |
| unset | delete a shortcut to an app |

  
### __set__ variables
* __project__ : the Convertigo project name holding the target application. This is Case sensitive
* __name__    : the shortcut name. If not provided the project name will be used automatically

### __custom__ variables
* __name__ : shortcut name used to redirect to the 'url'
* __url__  : absolute target URL for the redirect. Must be for this Convertigo server

### __unset__ variables
* __name__    : the shortcut name
  
## Note
If you want to create a shortcut to your app directly from an URL of this type 
`http(s)://<server>:<port>` so that just ascessing the Convertigo server starts a given app instead of the admin page. You can use the __set__ or __custom__ Sequences by providing explicitly the value 'index' for the __name__ variable.


