# &#10025; Summary

The global logger configuration.
Properties on this object can be changed during runtime and will affect logging of all components that are housed under the same root DI container as the logger.

| Modifier(s)                            | Extends                                    |
|----------------------------------------|--------------------------------------------|
| export | - |

# &#10025; Property(ies)

&nbsp;&nbsp; **&#10148; colorOptions**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

The global color options.

| Optional                           | Type                         |
|:----------------------------------:|------------------------------|
| ✘ | [ColorOptions](/kernel/enum/logger/coloroptions) |

&nbsp;&nbsp; **&#10148; level**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

The global log level. Only log calls with the same level or higher are emitted.

| Optional                           | Type                         |
|:----------------------------------:|------------------------------|
| ✘ | [LogLevel](/kernel/enum/reporter/loglevel) |