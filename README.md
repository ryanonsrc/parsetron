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
