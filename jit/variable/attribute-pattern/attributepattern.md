| Modifier(s)                            |
|----------------------------------------|
| export |

# &#9733; Variable(s)

&nbsp;&nbsp; **&#10148; AttributePattern**

| Type                        |
|-----------------------------|
| [AttributePattern](/jit/interface/attribute-pattern/attributepattern) |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Initializer**

```ts
Object.freeze({
  name: Protocol.resource.keyFor('attribute-pattern'),
  definitionAnnotationKey: 'attribute-pattern-definitions',
  define<TProto, TClass>(
    patternDefs: AttributePatternDefinition[],
    Type: DecoratableAttributePattern<TProto, TClass>,
      ) {
        validatePrototype(Type.prototype as IAttributePattern, patternDefs);
        const definition = new AttributePatternResourceDefinition(Type);
        const { name, definitionAnnotationKey } = AttributePattern;
        Metadata.define(name, definition, Type);
        Protocol.resource.appendTo(Type, name);
        Protocol.annotation.set(Type, definitionAnnotationKey, patternDefs);
        Protocol.annotation.appendTo(Type, definitionAnnotationKey);
        return Type as DecoratedAttributePattern<TProto, TClass>;
          },
          getPatternDefinitions<TProto, TClass>(Type: DecoratedAttributePattern<TProto, TClass>) {
            return Protocol.annotation.get(Type, AttributePattern.definitionAnnotationKey) as AttributePatternDefinition[];
          }
          })
```