# &#10025; Summary

A logging sink that emits `ILogEvent` objects to any kind of output. This can be the console, a database, a web api, a file, etc.
Multiple sinks can be registered, and all events will be emitted to all of them.

**Example**

// A buffered file sink that writes once per second:
```ts
export class BufferedFileSink {
  private readonly buffer: ILogEvent[] = [];
  constructor() {
    setInterval(() => {
      const events = this.buffer.splice(0);
      if (events.length > 0) {
        fs.appendFileSync('my-log.txt', events.map(e => e.toString()).join('\n'));
      }
    }, 1000);
  }
  public emit(event: ILogEvent): void {
    this.buffer.push(event);
  }
}
container.register(Registration.singleton(ISink, BufferedFileSink));
```

| Modifier(s)                            | Extends                                    |
|----------------------------------------|--------------------------------------------|
| export | - |

# &#10025; Method(s)

&nbsp;&nbsp; **&#10148; emit**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

Emit the provided `ILogEvent` to the output interface wrapped by this sink.

**Parameter(s)**

| Name  | Description                                                                                                                                      |
| ----- | ------------------------------------------------------------------------------------------------------------------------------------------------ |
| event |  The event object to emit. Built-in sinks will call `.toString()` on the event object but custom sinks can do anything they like with the event. |

| Return Type                       |
|-----------------------------------|
| void |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; event**_

| Modifier(s)                              | Optional                           | Rest                          | Parameter Property                          | Initializer                       |
|------------------------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|-----------------------------------|
| - | ✘  | ✘ | ✘ | - |