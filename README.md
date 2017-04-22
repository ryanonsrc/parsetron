parsetron - purely functional parser and AST generator
======

Adding to your application
------

```
resolvers ++= Seq(
    Resolver.sonatypeRepo("releases"),
    Resolver.sonatypeRepo("snapshots")
)

libraryDependencies ++= Seq(
    "io.nary" %% "parsetron" % "0.0.1"
)
```


Plan
------
Parse a script via atto and build an AST using Verizon quiver

script language:  LISP variant

syntax:

Call Expression:   (op arg1 arg2 ... argN)
Literal List:      [elm1 elm2 ... elmN]
Literal Set:       {elm1 elm2 ... elmN}
Define val:        <val lname value : body>
Define fun:        <fun lname arg1 arg2 ... argN impl : body>

Value types:
    lname
    Literals:
        "My String"
        1.23, .23, 0.23
        1, 5, 9999,
        true, false

