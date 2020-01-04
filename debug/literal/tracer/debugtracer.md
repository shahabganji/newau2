| Modifier(s)                            |
|----------------------------------------|
| export |

# &#9733; Literal(s)

&nbsp;&nbsp; **&#10148; DebugTracer**

| Type                        | Array                           |
|-----------------------------|---------------------------------|
| { enabled: boolean; liveLoggingEnabled: boolean; liveWriter: [ITraceWriter](/kernel/interface/reporter/itracewriter); enter(objName: string, methodName: string, args: unknown[] &#124; null): void; leave(): void; writeStack(writer: ITraceWriter): void; flushAll(writer: ITraceWriter &#124; null): void; enableLiveLogging: typeof enableLiveLogging; disableLiveLogging(): void; } | ✘ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Member(s)**

| Object                        |
|:-----------------------------:|
| ✔ |

**&#9733; Assignment(s)**

**&#10148; Tracer**

| Type                      | Shorthand                         | Spread                        |
|---------------------------|:---------------------------------:|:-----------------------------:|
| { enabled: false; liveLoggingEnabled: false; liveWriter: never; enter(objName: string, methodName: string, args: unknown[] &#124; null): void; leave(): void; writeStack(writer: [ITraceWriter](/kernel/interface/reporter/itracewriter)): void; flushAll(writer: ITraceWriter &#124; null): void; enableLiveLogging: typeof enableLiveLogging; disableLiveLogging(): void; } | ✘  | ✔ |

**&#9733; Value**

-

**&#10148; enabled**

| Type                      | Shorthand                         | Spread                        |
|---------------------------|:---------------------------------:|:-----------------------------:|
| { enabled: false; liveLoggingEnabled: false; liveWriter: never; enter(objName: string, methodName: string, args: unknown[] &#124; null): void; leave(): void; writeStack(writer: [ITraceWriter](/kernel/interface/reporter/itracewriter)): void; flushAll(writer: ITraceWriter &#124; null): void; enableLiveLogging: typeof enableLiveLogging; disableLiveLogging(): void; } | ✘  | ✘ |

**&#9733; Value**

false

**&#10148; liveLoggingEnabled**

| Type                      | Shorthand                         | Spread                        |
|---------------------------|:---------------------------------:|:-----------------------------:|
| { enabled: false; liveLoggingEnabled: false; liveWriter: never; enter(objName: string, methodName: string, args: unknown[] &#124; null): void; leave(): void; writeStack(writer: [ITraceWriter](/kernel/interface/reporter/itracewriter)): void; flushAll(writer: ITraceWriter &#124; null): void; enableLiveLogging: typeof enableLiveLogging; disableLiveLogging(): void; } | ✘  | ✘ |

**&#9733; Value**

false

**&#10148; liveWriter**

| Type                      | Shorthand                         | Spread                        |
|---------------------------|:---------------------------------:|:-----------------------------:|
| { enabled: false; liveLoggingEnabled: false; liveWriter: never; enter(objName: string, methodName: string, args: unknown[] &#124; null): void; leave(): void; writeStack(writer: [ITraceWriter](/kernel/interface/reporter/itracewriter)): void; flushAll(writer: ITraceWriter &#124; null): void; enableLiveLogging: typeof enableLiveLogging; disableLiveLogging(): void; } | ✘  | ✘ |

**&#9733; Value**

null!

**&#10148; enableLiveLogging**

| Type                      | Shorthand                         | Spread                        |
|---------------------------|:---------------------------------:|:-----------------------------:|
| { enabled: false; liveLoggingEnabled: false; liveWriter: never; enter(objName: string, methodName: string, args: unknown[] &#124; null): void; leave(): void; writeStack(writer: [ITraceWriter](/kernel/interface/reporter/itracewriter)): void; flushAll(writer: ITraceWriter &#124; null): void; enableLiveLogging: typeof enableLiveLogging; disableLiveLogging(): void; } | ✔  | ✘ |

**&#9733; Value**

-

**&#9733; Method(s)**

&nbsp;&nbsp; **&#10148; enter**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**;
Call this at the start of a method/function.
Each call to `enter` **must** have an accompanying call to `leave` for the tracer to work properly.

**Parameter(s)**

| Name       | Description                                                                                                                         |
| ---------- | ----------------------------------------------------------------------------------------------------------------------------------- |
| objName    |  Any human-friendly name to identify the traced object with.                                                                        |
| methodName |  Any human-friendly name to identify the traced method with.                                                                        |
| args       |  Pass in `Array.prototype.slice.call(arguments)` to also trace the parameters, or `null` if this is not needed (to save memory/cpu) |

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| - | ✘ | void |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; -**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          | Initializer                       |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|-----------------------------------|
| - | - | ✘  | ✘ | ✘ | - |

&nbsp;&nbsp; **&#10148; leave**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**;
Call this at the end of a method/function. Pops one trace item off the stack.

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| - | ✘ | void |

&nbsp;&nbsp; **&#10148; writeStack**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**;
Writes only the trace info leading up to the current method call.

**Parameter(s)**

| Name   | Description                        |
| ------ | ---------------------------------- |
| writer |  An object to write the output to. |

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| - | ✘ | void |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; -**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          | Initializer                       |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|-----------------------------------|
| - | - | ✘  | ✘ | ✘ | - |

&nbsp;&nbsp; **&#10148; flushAll**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**;
Writes all trace info captured since the previous flushAll operation.

**Parameter(s)**

| Name   | Description                                                                      |
| ------ | -------------------------------------------------------------------------------- |
| writer |  An object to write the output to. Can be null to simply reset the tracer state. |

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| - | ✘ | void |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; -**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          | Initializer                       |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|-----------------------------------|
| - | - | ✘  | ✘ | ✘ | - |

&nbsp;&nbsp; **&#10148; disableLiveLogging**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**;
Stops writing out each trace info item as they are traced.

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| - | ✘ | void |