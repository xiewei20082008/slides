---
theme : "white"
transition: "convex"
highlightTheme: "darkula"
---

# Functor, Monad and applicative

### Created by

Wei Xie

wei.xie@citrix.com
---

### Fmap

Schrodinger's interger

2 + 3 = 5

how about Schrodinger's 2

--

### Fmap

```ocaml
let schrodinger_2 =
    2 + 0/(mod tick 2)
```

--

### Fmap

```ocaml
type int Option
    | Some int
    | None
```

--

### Fmap

('a -> 'b) -> F 'a -> F 'b

---

### Monad

