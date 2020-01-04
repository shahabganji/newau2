| Modifier(s)                            |
|----------------------------------------|
| export |

# &#9733; Variable(s)

&nbsp;&nbsp; **&#10148; Profiler**

| Type                        |
|-----------------------------|
| { createTimer: (name: string) =&gt; [ITimer](/kernel/interface/profiler/itimer); enable: () =&gt; void; disable: () =&gt; void; report: (cb: (name: string, duration: number, topLevelCount: number, totalCount: number) =&gt; void) =&gt; void; readonly enabled: boolean; } |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Initializer**

```ts
(function (): {
  createTimer: typeof createTimer;
  enable: typeof enable;
  disable: typeof disable;
  report: typeof report;
  readonly enabled: boolean;
} {
  const now = PLATFORM.now;
  const timers: string[] = [];
  let profileMap: Record<string, IProfile>;
    const profiler = {
      createTimer,
      enable,
      disable,
      report,
      enabled: false
    };
    return profiler;
    function createTimer(name: string): ITimer {
      timers.push(name);
      let depth = 0;
      let mark = 0;
      return {
        enter,
        leave
      };
      function enter(): void {
        if (++depth === 1) {
          mark = now();
          ++profileMap[name].topLevelCount;
        }
        ++profileMap[name].totalCount;
      }
      function leave(): void {
        if (--depth === 0) {
          profileMap[name].duration += (now() - mark);
        }
      }
    }
    function enable(): void {
      profileMap = {};
      for (const timer of timers) {
        profileMap[timer] = {
          name: timer,
          duration: 0,
          topLevelCount: 0,
          totalCount: 0
        };
      }
      profiler.enabled = true;
    }
    function disable(): void {
      profiler.enabled = false;
    }
    function report(cb: (name: string, duration: number, topLevelCount: number, totalCount: number) => void): void {
      Object.keys(profileMap).map(key => profileMap[key]).sort((a, b) => b.duration - a.duration).forEach(p => {
        cb(p.name, p.duration, p.topLevelCount, p.totalCount);
      });
    }
    })()
```