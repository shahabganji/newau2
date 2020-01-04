| Modifier(s)                            | Extends                                    |
|----------------------------------------|--------------------------------------------|
| export | - |

# &#10025; Property(ies)

&nbsp;&nbsp; **&#10148; author**

| Optional                           | Type                         |
|:----------------------------------:|------------------------------|
| ✔ | string &#124; [PersonObject](/aot/system/interface/package-types/personobject) &#124; undefined |

&nbsp;&nbsp; **&#10148; bin**

| Optional                           | Type                         |
|:----------------------------------:|------------------------------|
| ✔ | string &#124; { [key: string]: string; } &#124; undefined |

&nbsp;&nbsp; **&#10148; bugs**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

The url to your project's issue tracker and / or the email address to which issues should
be reported. These are helpful for people who encounter issues with your package.

| Optional                           | Type                         |
|:----------------------------------:|------------------------------|
| ✔ | string &#124; [BugsObject](/aot/system/interface/package-types/bugsobject) &#124; undefined |

&nbsp;&nbsp; **&#10148; config**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

A 'config' hash can be used to set configuration parameters used in package scripts that
persist across upgrades.

| Optional                           | Type                         |
|:----------------------------------:|------------------------------|
| ✔ | { [key: string]: any; } &#124; undefined |

&nbsp;&nbsp; **&#10148; contributors**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

A list of people who contributed to this package.

| Optional                           | Type                         |
|:----------------------------------:|------------------------------|
| ✔ | (string &#124; [PersonObject](/aot/system/interface/package-types/personobject))[] &#124; undefined |

&nbsp;&nbsp; **&#10148; cpu**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

If your code only runs on certain cpu architectures, you can specify which ones.

| Optional                           | Type                         |
|:----------------------------------:|------------------------------|
| ✔ | string[] &#124; undefined |

&nbsp;&nbsp; **&#10148; dependencies**

| Optional                           | Type                         |
|:----------------------------------:|------------------------------|
| ✔ | { [key: string]: string; } &#124; undefined |

&nbsp;&nbsp; **&#10148; description**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

This helps people discover your package, as it's listed in 'npm search'.

| Optional                           | Type                         |
|:----------------------------------:|------------------------------|
| ✔ | string &#124; undefined |

&nbsp;&nbsp; **&#10148; devDependencies**

| Optional                           | Type                         |
|:----------------------------------:|------------------------------|
| ✔ | { [key: string]: string; } &#124; undefined |

&nbsp;&nbsp; **&#10148; directories**

| Optional                           | Type                         |
|:----------------------------------:|------------------------------|
| ✔ | [Directories](/aot/system/interface/package-types/directories) &#124; undefined |

&nbsp;&nbsp; **&#10148; dist**

| Optional                           | Type                         |
|:----------------------------------:|------------------------------|
| ✔ | [Dist](/aot/system/interface/package-types/dist) &#124; undefined |

&nbsp;&nbsp; **&#10148; engines**

| Optional                           | Type                         |
|:----------------------------------:|------------------------------|
| ✔ | { [key: string]: string; } &#124; undefined |

&nbsp;&nbsp; **&#10148; engineStrict**

| Optional                           | Type                         |
|:----------------------------------:|------------------------------|
| ✔ | boolean &#124; undefined |

&nbsp;&nbsp; **&#10148; esnext**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

A module ID with untranspiled code that is the primary entry point to your program.

| Optional                           | Type                         |
|:----------------------------------:|------------------------------|
| ✔ | string &#124; [EsnextObject](/aot/system/interface/package-types/esnextobject) &#124; undefined |

&nbsp;&nbsp; **&#10148; files**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

The 'files' field is an array of files to include in your project. If you name a folder
in the array, then it will also include the files inside that folder.

| Optional                           | Type                         |
|:----------------------------------:|------------------------------|
| ✔ | string[] &#124; undefined |

&nbsp;&nbsp; **&#10148; homepage**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

The url to the project homepage.

| Optional                           | Type                         |
|:----------------------------------:|------------------------------|
| ✔ | string &#124; undefined |

&nbsp;&nbsp; **&#10148; keywords**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

This helps people discover your package as it's listed in 'npm search'.

| Optional                           | Type                         |
|:----------------------------------:|------------------------------|
| ✔ | string[] &#124; undefined |

&nbsp;&nbsp; **&#10148; license**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

You should specify a license for your package so that people know how they are permitted
to use it, and any restrictions you're placing on it.

| Optional                           | Type                         |
|:----------------------------------:|------------------------------|
| ✔ | string &#124; undefined |

&nbsp;&nbsp; **&#10148; licenses**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

You should specify a license for your package so that people know how they are permitted
to use it, and any restrictions you're placing on it.

| Optional                           | Type                         |
|:----------------------------------:|------------------------------|
| ✔ | [License](/aot/system/interface/package-types/license)[] &#124; undefined |

&nbsp;&nbsp; **&#10148; main**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

The main field is a module ID that is the primary entry point to your program.

| Optional                           | Type                         |
|:----------------------------------:|------------------------------|
| ✔ | string &#124; undefined |

&nbsp;&nbsp; **&#10148; maintainers**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

A list of people who maintains this package.

| Optional                           | Type                         |
|:----------------------------------:|------------------------------|
| ✔ | (string &#124; [PersonObject](/aot/system/interface/package-types/personobject))[] &#124; undefined |

&nbsp;&nbsp; **&#10148; man**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

Specify either a single file or an array of filenames to put in place for the man program
to find.

| Optional                           | Type                         |
|:----------------------------------:|------------------------------|
| ✔ | string &#124; string[] &#124; undefined |

&nbsp;&nbsp; **&#10148; module**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

An ECMAScript module ID that is the primary entry point to your program.

| Optional                           | Type                         |
|:----------------------------------:|------------------------------|
| ✔ | string &#124; undefined |

&nbsp;&nbsp; **&#10148; name**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

The name of the package.

| Optional                           | Type                         |
|:----------------------------------:|------------------------------|
| ✔ | string &#124; undefined |

&nbsp;&nbsp; **&#10148; optionalDependencies**

| Optional                           | Type                         |
|:----------------------------------:|------------------------------|
| ✔ | { [key: string]: string; } &#124; undefined |

&nbsp;&nbsp; **&#10148; os**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

You can specify which operating systems your module will run on

| Optional                           | Type                         |
|:----------------------------------:|------------------------------|
| ✔ | string[] &#124; undefined |

&nbsp;&nbsp; **&#10148; peerDependencies**

| Optional                           | Type                         |
|:----------------------------------:|------------------------------|
| ✔ | { [key: string]: string; } &#124; undefined |

&nbsp;&nbsp; **&#10148; preferGlobal**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

If your package is primarily a command-line application that should be installed
globally, then set this value to true to provide a warning if it is installed locally.

| Optional                           | Type                         |
|:----------------------------------:|------------------------------|
| ✔ | boolean &#124; undefined |

&nbsp;&nbsp; **&#10148; private**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

If set to true, then npm will refuse to publish it.

| Optional                           | Type                         |
|:----------------------------------:|------------------------------|
| ✔ | boolean &#124; undefined |

&nbsp;&nbsp; **&#10148; publishConfig**

| Optional                           | Type                         |
|:----------------------------------:|------------------------------|
| ✔ | { [key: string]: any; } &#124; undefined |

&nbsp;&nbsp; **&#10148; readme**

| Optional                           | Type                         |
|:----------------------------------:|------------------------------|
| ✔ | string &#124; undefined |

&nbsp;&nbsp; **&#10148; repository**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

Specify the place where your code lives. This is helpful for people who want to
contribute.

| Optional                           | Type                         |
|:----------------------------------:|------------------------------|
| ✔ | string &#124; [RepositoryObject](/aot/system/interface/package-types/repositoryobject) &#124; undefined |

&nbsp;&nbsp; **&#10148; scripts**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

The 'scripts' member is an object hash of script commands that are run at various times
in the lifecycle of your package. The key is the lifecycle event, and the value is the
command to run at that point.

| Optional                           | Type                         |
|:----------------------------------:|------------------------------|
| ✔ | [Scripts](/aot/system/interface/package-types/scripts) &#124; undefined |

&nbsp;&nbsp; **&#10148; version**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

Version must be parseable by node-semver, which is bundled with npm as a dependency.

| Optional                           | Type                         |
|:----------------------------------:|------------------------------|
| ✔ | string &#124; undefined |