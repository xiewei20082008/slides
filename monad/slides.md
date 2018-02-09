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
type option
    | Some of int
    | None
```

--

### Fmap

* fmap (<$>)

('a -> 'b) -> F 'a -> F 'b

---

### Monad

* bind 

('a -> M 'b) -> (M 'a) -> M 'b

let (>>=) m f = bind f m

* \>\>=

(M 'a) -> ('a -> M 'b) -> M 'b

--

### Monad

A monad in X is just a monoid in the category of endofunctors of X, with product × replaced by composition of endofunctors and unit set by the identity endofunctor.

---

### Applicative

A ('a -> 'b) -> F 'a -> F 'b

---

### Failure handling

* exception
    * Go To Statement Considered Harmful
* error as return value

https://github.com/xenserver/xe-guest-utilities/blob/master/guestmetric/guestmetric_linux.go#L122

https://github.com/xapi-project/xcp-networkd/blob/sr-iov/networkd/network_server.ml#L249



