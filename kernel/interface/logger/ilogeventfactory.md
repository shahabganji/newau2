# &#10025; Summary

Component that creates log event objects based on raw inputs sent to `ILogger`.
To customize what data is sent to the sinks, replace the implementation for this interface with your own.

**Example**

```ts
export class MyLogEventFactory {
  public createLogEvent(logger: ILogger, logLevel: LogLevel, message: string, optionalParams: unknown[]): ILogEvent {
    return {
      logLevel,
      optionalParams,
      toString() {
        return `[${logger.scope.join('.')}] ${message} ${optionalParams.join(', ')}`;
      }
    };
  }
}
container.register(Registration.singleton(ILogEventFactory, MyLogEventFactory));
```

| Modifier(s)                            | Extends                                    |
|----------------------------------------|--------------------------------------------|
| export | - |

# &#10025; Method(s)

&nbsp;&nbsp; **&#10148; createLogEvent**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

Create a log event object based on the input parameters sent to `ILogger`.

**Parameter(s)**

| Name           | Description                                                                                                                                               |
| -------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------- |
| logger         |  The `ILogger` that received the message.                                                                                                                 |
| logLevel       |  The `LogLevel` associated with the `ILogger` method that the message was passed into. E.g. `logger.debug` will result in `LogLevel.debug`                |
| message        |  The message (first parameter) that was passed into the logger. If a function was passed into the logger, this will be the return value of that function. |
| optionalParams |  Additional optional parameters there were passed into the logger, if any.                                                                                |

**Returns**

An `ILogEvent` object that, by default, only has a `.toString()` method.
This is called by the default console sink to get the message to emit to the console.
It could be any object of any shape, as long as the registered sinks understand that shape.

| Return Type                       |
|-----------------------------------|
| [ILogEvent](/kernel/interface/logger/ilogevent) |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; logger**_

| Modifier(s)                              | Optional                           | Rest                          | Parameter Property                          | Initializer                       |
|------------------------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|-----------------------------------|
| - | ✘  | ✘ | ✘ | - |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; logLevel**_

| Modifier(s)                              | Optional                           | Rest                          | Parameter Property                          | Initializer                       |
|------------------------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|-----------------------------------|
| - | ✘  | ✘ | ✘ | - |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; message**_

| Modifier(s)                              | Optional                           | Rest                          | Parameter Property                          | Initializer                       |
|------------------------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|-----------------------------------|
| - | ✘  | ✘ | ✘ | - |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; optionalParams**_

| Modifier(s)                              | Optional                           | Rest                          | Parameter Property                          | Initializer                       |
|------------------------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|-----------------------------------|
| - | ✘  | ✘ | ✘ | - |