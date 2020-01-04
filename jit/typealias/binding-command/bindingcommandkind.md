| Modifier(s)                            | Type                     |
|----------------------------------------|--------------------------|
| export | BindingCommandKind |

# &#10025; Initializer

```ts
IResourceKind<BindingCommandType, BindingCommandDefinition> & {
  isType<T>(value: T): value is (T extends Constructable ? BindingCommandType<T> : never);
    define<T extends Constructable>(name: string, Type: T): BindingCommandType<T>;
      define<T extends Constructable>(def: PartialBindingCommandDefinition, Type: T): BindingCommandType<T>;
        define<T extends Constructable>(nameOrDef: string | PartialBindingCommandDefinition, Type: T): BindingCommandType<T>;
          getDefinition<T extends Constructable>(Type: T): BindingCommandDefinition<T>;
            annotate<K extends keyof PartialBindingCommandDefinition>(Type: Constructable, prop: K, value: PartialBindingCommandDefinition[K]): void;
              getAnnotation<K extends keyof PartialBindingCommandDefinition>(Type: Constructable, prop: K): PartialBindingCommandDefinition[K];
                }
```