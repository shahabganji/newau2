# &#10025; Summary

The main interface to the logging API.
Inject this as a dependency in your components to add centralized, configurable logging capabilities to your application.

| Modifier(s)                            | Extends                                    |
|----------------------------------------|--------------------------------------------|
| export | - |

# &#10025; Property(ies)

&nbsp;&nbsp; **&#10148; root**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

The root `ILogger` instance. On the root logger itself, this property circularly references the root. It is never null.
When using `.scopeTo`, a new `ILogger` is created. That new logger will have the `root` property set to the global (non-scoped) logger.

| Optional                           | Type                         |
|:----------------------------------:|------------------------------|
| ✘ | [ILogger](/kernel/interface/logger/ilogger) |

&nbsp;&nbsp; **&#10148; parent**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

The parent `ILogger` instance. On the root logger itself, this property circularly references the root. It is never null.
When using `.scopeTo`, a new `ILogger` is created. That new logger will have the `parent` property set to the logger that it was created from.

| Optional                           | Type                         |
|:----------------------------------:|------------------------------|
| ✘ | [ILogger](/kernel/interface/logger/ilogger) |

&nbsp;&nbsp; **&#10148; scope**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

The scopes that this logger was created for, if any.

| Optional                           | Type                         |
|:----------------------------------:|------------------------------|
| ✘ | readonly string[] |

&nbsp;&nbsp; **&#10148; config**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

The global logger configuration.

| Optional                           | Type                         |
|:----------------------------------:|------------------------------|
| ✘ | [ILogConfig](/kernel/interface/logger/ilogconfig) |

# &#10025; Method(s)

&nbsp;&nbsp; **&#10148; trace**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

Write to TRC output, if the configured `LogLevel` is set to `trace`.
Intended for the most detailed information about internal app state.

**Parameter(s)**

| Name           | Description                                                                                                                                                                                                                                                                   |
| -------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| getMessage     |  A function to build the message to pass to the `ILogEventFactory`. Only called if the configured `LogLevel` dictates that these messages be emitted. Use this when creating the log message is potentially expensive and should only be done if the log is actually emitted. |
| optionalParams |  Any additional, optional params that should be passed to the `ILogEventFactory`                                                                                                                                                                                              |

| Return Type                       |
|-----------------------------------|
| void |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; getMessage**_

| Modifier(s)                              | Optional                           | Rest                          | Parameter Property                          | Initializer                       |
|------------------------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|-----------------------------------|
| - | ✘  | ✘ | ✘ | - |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; optionalParams**_

| Modifier(s)                              | Optional                           | Rest                          | Parameter Property                          | Initializer                       |
|------------------------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|-----------------------------------|
| - | ✔  | ✔ | ✘ | - |

&nbsp;&nbsp; **&#10148; trace**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

Write to TRC output, if the configured `LogLevel` is set to `trace`.
Intended for the most detailed information about internal app state.

**Parameter(s)**

| Name           | Description                                                                      |
| -------------- | -------------------------------------------------------------------------------- |
| message        |  The message to pass to the `ILogEventFactory`.                                  |
| optionalParams |  Any additional, optional params that should be passed to the `ILogEventFactory` |

| Return Type                       |
|-----------------------------------|
| void |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; message**_

| Modifier(s)                              | Optional                           | Rest                          | Parameter Property                          | Initializer                       |
|------------------------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|-----------------------------------|
| - | ✘  | ✘ | ✘ | - |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; optionalParams**_

| Modifier(s)                              | Optional                           | Rest                          | Parameter Property                          | Initializer                       |
|------------------------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|-----------------------------------|
| - | ✔  | ✔ | ✘ | - |

&nbsp;&nbsp; **&#10148; debug**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

Write to DBG output, if the configured `LogLevel` is set to `debug` or lower.
Intended for information that is useful for debugging during development and has no long-term value.

**Parameter(s)**

| Name           | Description                                                                                                                                                                                                                                                                   |
| -------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| getMessage     |  A function to build the message to pass to the `ILogEventFactory`. Only called if the configured `LogLevel` dictates that these messages be emitted. Use this when creating the log message is potentially expensive and should only be done if the log is actually emitted. |
| optionalParams |  Any additional, optional params that should be passed to the `ILogEventFactory`                                                                                                                                                                                              |

| Return Type                       |
|-----------------------------------|
| void |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; getMessage**_

| Modifier(s)                              | Optional                           | Rest                          | Parameter Property                          | Initializer                       |
|------------------------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|-----------------------------------|
| - | ✘  | ✘ | ✘ | - |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; optionalParams**_

| Modifier(s)                              | Optional                           | Rest                          | Parameter Property                          | Initializer                       |
|------------------------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|-----------------------------------|
| - | ✔  | ✔ | ✘ | - |

&nbsp;&nbsp; **&#10148; debug**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

Write to DBG output, if the configured `LogLevel` is set to `debug` or lower.
Intended for information that is useful for debugging during development and has no long-term value.

**Parameter(s)**

| Name           | Description                                                                      |
| -------------- | -------------------------------------------------------------------------------- |
| message        |  The message to pass to the `ILogEventFactory`.                                  |
| optionalParams |  Any additional, optional params that should be passed to the `ILogEventFactory` |

| Return Type                       |
|-----------------------------------|
| void |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; message**_

| Modifier(s)                              | Optional                           | Rest                          | Parameter Property                          | Initializer                       |
|------------------------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|-----------------------------------|
| - | ✘  | ✘ | ✘ | - |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; optionalParams**_

| Modifier(s)                              | Optional                           | Rest                          | Parameter Property                          | Initializer                       |
|------------------------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|-----------------------------------|
| - | ✔  | ✔ | ✘ | - |

&nbsp;&nbsp; **&#10148; info**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

Write to trace UBF, if the configured `LogLevel` is set to `info` or lower.
Intended for information about the general flow of the application that has long-term value.

**Parameter(s)**

| Name           | Description                                                                                                                                                                                                                                                                   |
| -------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| getMessage     |  A function to build the message to pass to the `ILogEventFactory`. Only called if the configured `LogLevel` dictates that these messages be emitted. Use this when creating the log message is potentially expensive and should only be done if the log is actually emitted. |
| optionalParams |  Any additional, optional params that should be passed to the `ILogEventFactory`                                                                                                                                                                                              |

| Return Type                       |
|-----------------------------------|
| void |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; getMessage**_

| Modifier(s)                              | Optional                           | Rest                          | Parameter Property                          | Initializer                       |
|------------------------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|-----------------------------------|
| - | ✘  | ✘ | ✘ | - |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; optionalParams**_

| Modifier(s)                              | Optional                           | Rest                          | Parameter Property                          | Initializer                       |
|------------------------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|-----------------------------------|
| - | ✔  | ✔ | ✘ | - |

&nbsp;&nbsp; **&#10148; info**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

Write to trace UBF, if the configured `LogLevel` is set to `info` or lower.
Intended for information about the general flow of the application that has long-term value.

**Parameter(s)**

| Name           | Description                                                                      |
| -------------- | -------------------------------------------------------------------------------- |
| message        |  The message to pass to the `ILogEventFactory`.                                  |
| optionalParams |  Any additional, optional params that should be passed to the `ILogEventFactory` |

| Return Type                       |
|-----------------------------------|
| void |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; message**_

| Modifier(s)                              | Optional                           | Rest                          | Parameter Property                          | Initializer                       |
|------------------------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|-----------------------------------|
| - | ✘  | ✘ | ✘ | - |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; optionalParams**_

| Modifier(s)                              | Optional                           | Rest                          | Parameter Property                          | Initializer                       |
|------------------------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|-----------------------------------|
| - | ✔  | ✔ | ✘ | - |

&nbsp;&nbsp; **&#10148; warn**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

Write to WRN output, if the configured `LogLevel` is set to `warn` or lower.
Intended for unexpected circumstances that require attention but do not otherwise cause the current flow of execution to stop.

**Parameter(s)**

| Name           | Description                                                                                                                                                                                                                                                                   |
| -------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| getMessage     |  A function to build the message to pass to the `ILogEventFactory`. Only called if the configured `LogLevel` dictates that these messages be emitted. Use this when creating the log message is potentially expensive and should only be done if the log is actually emitted. |
| optionalParams |  Any additional, optional params that should be passed to the `ILogEventFactory`                                                                                                                                                                                              |

| Return Type                       |
|-----------------------------------|
| void |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; getMessage**_

| Modifier(s)                              | Optional                           | Rest                          | Parameter Property                          | Initializer                       |
|------------------------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|-----------------------------------|
| - | ✘  | ✘ | ✘ | - |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; optionalParams**_

| Modifier(s)                              | Optional                           | Rest                          | Parameter Property                          | Initializer                       |
|------------------------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|-----------------------------------|
| - | ✔  | ✔ | ✘ | - |

&nbsp;&nbsp; **&#10148; warn**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

Write to WRN output, if the configured `LogLevel` is set to `warn` or lower.
Intended for unexpected circumstances that require attention but do not otherwise cause the current flow of execution to stop.

**Parameter(s)**

| Name           | Description                                                                      |
| -------------- | -------------------------------------------------------------------------------- |
| message        |  The message to pass to the `ILogEventFactory`.                                  |
| optionalParams |  Any additional, optional params that should be passed to the `ILogEventFactory` |

| Return Type                       |
|-----------------------------------|
| void |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; message**_

| Modifier(s)                              | Optional                           | Rest                          | Parameter Property                          | Initializer                       |
|------------------------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|-----------------------------------|
| - | ✘  | ✘ | ✘ | - |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; optionalParams**_

| Modifier(s)                              | Optional                           | Rest                          | Parameter Property                          | Initializer                       |
|------------------------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|-----------------------------------|
| - | ✔  | ✔ | ✘ | - |

&nbsp;&nbsp; **&#10148; error**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

Write to ERR output, if the configured `LogLevel` is set to `error` or lower.
Intended for unexpected circumstances that cause the flow of execution in the current activity to stop but do not cause an app-wide failure.

**Parameter(s)**

| Name           | Description                                                                                                                                                                                                                                                                   |
| -------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| getMessage     |  A function to build the message to pass to the `ILogEventFactory`. Only called if the configured `LogLevel` dictates that these messages be emitted. Use this when creating the log message is potentially expensive and should only be done if the log is actually emitted. |
| optionalParams |  Any additional, optional params that should be passed to the `ILogEventFactory`                                                                                                                                                                                              |

| Return Type                       |
|-----------------------------------|
| void |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; getMessage**_

| Modifier(s)                              | Optional                           | Rest                          | Parameter Property                          | Initializer                       |
|------------------------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|-----------------------------------|
| - | ✘  | ✘ | ✘ | - |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; optionalParams**_

| Modifier(s)                              | Optional                           | Rest                          | Parameter Property                          | Initializer                       |
|------------------------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|-----------------------------------|
| - | ✔  | ✔ | ✘ | - |

&nbsp;&nbsp; **&#10148; error**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

Write to ERR output, if the configured `LogLevel` is set to `error` or lower.
Intended for unexpected circumstances that cause the flow of execution in the current activity to stop but do not cause an app-wide failure.

**Parameter(s)**

| Name           | Description                                                                      |
| -------------- | -------------------------------------------------------------------------------- |
| message        |  The message to pass to the `ILogEventFactory`.                                  |
| optionalParams |  Any additional, optional params that should be passed to the `ILogEventFactory` |

| Return Type                       |
|-----------------------------------|
| void |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; message**_

| Modifier(s)                              | Optional                           | Rest                          | Parameter Property                          | Initializer                       |
|------------------------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|-----------------------------------|
| - | ✘  | ✘ | ✘ | - |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; optionalParams**_

| Modifier(s)                              | Optional                           | Rest                          | Parameter Property                          | Initializer                       |
|------------------------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|-----------------------------------|
| - | ✔  | ✔ | ✘ | - |

&nbsp;&nbsp; **&#10148; fatal**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

Write to FTL output, if the configured `LogLevel` is set to `fatal` or lower.
Intended for unexpected circumstances that cause an app-wide failure or otherwise require immediate attention.

**Parameter(s)**

| Name           | Description                                                                                                                                                                                                                                                                   |
| -------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| getMessage     |  A function to build the message to pass to the `ILogEventFactory`. Only called if the configured `LogLevel` dictates that these messages be emitted. Use this when creating the log message is potentially expensive and should only be done if the log is actually emitted. |
| optionalParams |  Any additional, optional params that should be passed to the `ILogEventFactory`                                                                                                                                                                                              |

| Return Type                       |
|-----------------------------------|
| void |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; getMessage**_

| Modifier(s)                              | Optional                           | Rest                          | Parameter Property                          | Initializer                       |
|------------------------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|-----------------------------------|
| - | ✘  | ✘ | ✘ | - |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; optionalParams**_

| Modifier(s)                              | Optional                           | Rest                          | Parameter Property                          | Initializer                       |
|------------------------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|-----------------------------------|
| - | ✔  | ✔ | ✘ | - |

&nbsp;&nbsp; **&#10148; fatal**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

Write to FTL output, if the configured `LogLevel` is set to `fatal` or lower.
Intended for unexpected circumstances that cause an app-wide failure or otherwise require immediate attention.

**Parameter(s)**

| Name           | Description                                                                      |
| -------------- | -------------------------------------------------------------------------------- |
| message        |  The message to pass to the `ILogEventFactory`.                                  |
| optionalParams |  Any additional, optional params that should be passed to the `ILogEventFactory` |

| Return Type                       |
|-----------------------------------|
| void |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; message**_

| Modifier(s)                              | Optional                           | Rest                          | Parameter Property                          | Initializer                       |
|------------------------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|-----------------------------------|
| - | ✘  | ✘ | ✘ | - |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; optionalParams**_

| Modifier(s)                              | Optional                           | Rest                          | Parameter Property                          | Initializer                       |
|------------------------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|-----------------------------------|
| - | ✔  | ✔ | ✘ | - |

&nbsp;&nbsp; **&#10148; scopeTo**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

Create a new logger with an additional permanent prefix added to the logging outputs.
When chained, multiple scopes are separated by a dot.
This is preliminary API and subject to change before alpha release.

**Example**

```ts
export class MyComponent {
  constructor(
    
    **Ilogger**
    
    private logger: ILogger) {
    this.logger.debug('before scoping');
    // console output: '[DBG] before scoping'
    this.logger = logger.scopeTo('MyComponent');
    this.logger.debug('after scoping');
    // console output: '[DBG MyComponent] after scoping'
  }
  public doStuff(): void {
    const logger = this.logger.scopeTo('doStuff()');
    logger.debug('doing stuff');
    // console output: '[DBG MyComponent.doStuff()] doing stuff'
  }
}
```

| Return Type                       |
|-----------------------------------|
| [ILogger](/kernel/interface/logger/ilogger) |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; name**_

| Modifier(s)                              | Optional                           | Rest                          | Parameter Property                          | Initializer                       |
|------------------------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|-----------------------------------|
| - | ✘  | ✘ | ✘ | - |