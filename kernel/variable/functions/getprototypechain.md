| Modifier(s)                            |
|----------------------------------------|
| export |

# &#9733; Variable(s)

&nbsp;&nbsp; **&#10148; getPrototypeChain**

| Type                        |
|-----------------------------|
| &lt;T extends Constructable&lt;{}&gt;&gt;(Type: T) =&gt; readonly [T, ...Constructable&lt;{}&gt;[]] |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Initializer**

```ts
(function () {
  const functionPrototype = Function.prototype;
  // eslint-disable-next-line @typescript-eslint/unbound-method
  const getPrototypeOf = Object.getPrototypeOf;
  const cache = new WeakMap<Constructable, [Constructable, ...Constructable[]]>();
    let proto = functionPrototype as Constructable;
    let i = 0;
    let chain: [Constructable, ...Constructable[]] | undefined = void 0;
    return function <T extends Constructable> (Type: T): readonly [T, ...Constructable[]] {
      chain = cache.get(Type);
      if (chain === void 0) {
        cache.set(Type, chain = [proto = Type]);
        i = 0;
        while ((proto = getPrototypeOf(proto)) !== functionPrototype) {
          chain[++i] = proto;
        }
      }
      return chain as [T, ...Constructable[]];
    };
    })()
```