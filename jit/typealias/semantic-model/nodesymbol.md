| Modifier(s)                            | Type                     |
|----------------------------------------|--------------------------|
| export | NodeSymbol&lt;TText, TElement, TMarker&gt; |

# &#10025; Type Parameter(s)

| Type  | Constraint                            |
| ----- | ------------------------------------- |
| TText | [INode](/runtime/interface/dom/inode) |

| Type     | Constraint                            |
| -------- | ------------------------------------- |
| TElement | [INode](/runtime/interface/dom/inode) |

| Type    | Constraint                            |
| ------- | ------------------------------------- |
| TMarker | [INode](/runtime/interface/dom/inode) |

# &#10025; Initializer

```ts
(
  CustomElementSymbol<TText, TElement, TMarker> |
    LetElementSymbol<TElement, TMarker> |
      PlainElementSymbol<TText, TElement, TMarker> |
        ReplacePartSymbol<TText, TElement, TMarker> |
          TemplateControllerSymbol<TText, TElement, TMarker> |
            TextSymbol<TText, TMarker>
              )
```