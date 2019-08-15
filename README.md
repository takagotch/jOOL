### jool
---
https://github.com/jOOQ/jOOL

```java
Arrays.stream(dir.listFiles()).forEach(file -> {
  try {
    System.out.println(file.getCanonicalPath());
  }
  catch (IOException e) {
    throw new RuntimeException(e);
  }
});

Arrays.stream(dir.listFiles()).forEach(
  Unchecked.consumer(file -> { System.out.println(file.getCannonicalPath(); )})
);

Arrays.stream(dir.listFiles())
  .map(Unchecked.function(File::getCannonicalPath))
  .forEach(System.out::println);
  
Unchecked.throwChecked(new Exception());

Seq.of(1, 2, 3).concat(Seq.of(4, 5, 6));
Seq.of(1, 2, 3, 4).contains(2);
```

```
```

```
```
