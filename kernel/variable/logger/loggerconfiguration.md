# &#9733; Summary

A basic `ILogger` configuration that configures a single `console` sink based on provided options.
NOTE: You *must* register the return value of `.create` with the container / au instance, not this `LoggerConfiguration` object itself.
```ts
// GOOD
container.register(LoggerConfiguration.create(console))
// GOOD
container.register(LoggerConfiguration.create(console, LogLevel.debug))
// GOOD
container.register(LoggerConfiguration.create({
  debug: PLATFORM.noop,
  info: PLATFORM.noop,
  warn: PLATFORM.noop,
  error: msg => {
    throw new Error(msg);
  }
}, LogLevel.debug))
// BAD
container.register(LoggerConfiguration)
```

| Modifier(s)                            |
|----------------------------------------|
| export |

# &#9733; Variable(s)

&nbsp;&nbsp; **&#10148; LoggerConfiguration**

| Type                        |
|-----------------------------|
| { create($console: [IConsoleLike](/kernel/interface/logger/iconsolelike), level?: [LogLevel](/kernel/enum/reporter/loglevel), colorOptions?: [ColorOptions](/kernel/enum/logger/coloroptions)): [IRegistry](/kernel/interface/di/iregistry); } |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Initializer**

```ts
toLookup({
  
  /**

* @param $console - The `console` object to use. Can be the native `window.console` / `global.console`, but can also be a wrapper or mock that implements the same interface.
* @param level - The global `LogLevel` to configure. Defaults to `warn` or higher.
* @param colorOptions - Whether to use colors or not. Defaults to `noColors`. Colors are especially nice in nodejs environments but don't necessarily work (well) in all environments, such as browsers.
  */
  create(
    $console: IConsoleLike,
    level: LogLevel = LogLevel.warn,
      colorOptions = ColorOptions.noColors,
      ): IRegistry {
        return toLookup({
          register(container: IContainer): IContainer {
            return container.register(
              Registration.instance(ILogConfig, new LogConfig(colorOptions, level)),
              Registration.instance(ISink, new ConsoleSink($console)),
            );
          },
        });
      },
      })
```