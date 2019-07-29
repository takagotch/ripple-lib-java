### ripple-lib-java
---
https://github.com/ripple-unmaintained/ripple-lib-java

```java
// src/.

protected abstract static class STArrayField implements HasField{}
public static STArrayField starrayField(final Field f) {
  return new STArrayField() { @Override public Field getField() {return f;}};
}

static public STArrayField AffectedNodes = starrayField(Field.AffectedNodes);
static public STArrayField Signatures = starrayField(Field.Signatures);
static public STArrayField Template = starrayField(Field.Tmplate);

if (transactionType() == TransactionType.Payment && meta.has(STArray.AffectedNodes)) {
  STArray affected = meta.get(STArray.AffectedNodes);
  for (STObject node : affected) {
    if (node.has(STObject.CreatedNode)) {
      STObject created = node.get(STObject.CreatedNode);
    }
  }
}

public STArray get(STArray.STArrayField f) {
  return (STArray) fields.get(f.getField());
}

public interface SerializedType {
  Object toJSON();
  byte[] toBytes();
  String toHext();
  void toBytesSink(ByteSink to);
}

so = STObject()
so.name = "FileName"
so["FieldOfDreams"] = "A Kevin Costner Movie"
sa = STArray([so])
```

```
```

```
```


