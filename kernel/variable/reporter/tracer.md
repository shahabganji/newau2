| Modifier(s)                            |
|----------------------------------------|
| export |

# &#9733; Variable(s)

&nbsp;&nbsp; **&#10148; Tracer**

| Type                        |
|-----------------------------|
| { enabled: boolean; liveLoggingEnabled: boolean; liveWriter: [ITraceWriter](/kernel/interface/reporter/itracewriter); enter(objName: string, methodName: string, args: unknown[] &#124; null): void; leave(): void; writeStack(writer: ITraceWriter): void; flushAll(writer: ITraceWriter &#124; null): void; enableLiveLogging: typeof enableLiveLogging; disableLiveLogging(): void; } |