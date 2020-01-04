| Modifier(s)                            |
|----------------------------------------|
| export |

# &#9733; Variable(s)

&nbsp;&nbsp; **&#10148; Registration**

| Type                        |
|-----------------------------|
| Readonly&lt;{ instance&lt;T&gt;(key: Key, value: T): [IRegistration](/kernel/interface/di/iregistration)&lt;T&gt;; singleton&lt;T&#95;1 extends Constructable&lt;{}&gt;&gt;(key: Key, value: T&#95;1): IRegistration&lt;InstanceType&lt;T&#95;1&gt;&gt;; transient&lt;T&#95;2 extends Constructable&lt;{}&gt;&gt;(key: Key, value: T&#95;2): IRegistration&lt;InstanceType&lt;T&#95;2&gt;&gt;; callback&lt;T&#95;3&gt;(key: Key, callback: ResolveCallback&lt;T&#95;3&gt;): IRegistration&lt;T&#95;3 extends InterfaceSymbol&lt;infer T&#95;4&gt; ? T&#95;4 : T&#95;3 extends Constructable&lt;{}&gt; ? InstanceType&lt;T&#95;3&gt; : T&#95;3 extends IResolverLike&lt;infer T1, any&gt; ? T1 extends Constructable&lt;{}&gt; ? InstanceType&lt;T1&gt; : T1 : T&#95;3&gt;; alias&lt;T&#95;5&gt;(originalKey: T&#95;5, aliasKey: Key): IRegistration&lt;T&#95;5 extends InterfaceSymbol&lt;infer T&#95;4&gt; ? T&#95;4 : T&#95;5 extends Constructable&lt;{}&gt; ? InstanceType&lt;T&#95;5&gt; : T&#95;5 extends IResolverLike&lt;infer T1, any&gt; ? T1 extends Constructable&lt;{}&gt; ? InstanceType&lt;T1&gt; : T1 : T&#95;5&gt;; defer(key: Key, ...params: unknown[]): [IRegistry](/kernel/interface/di/iregistry); }&gt; |