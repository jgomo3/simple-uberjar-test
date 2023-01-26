# simple-uberjar-test

You could run this project simply with Clojure, and it should print HOLA:

```
$ clojure -M -m my.lib
HOLA
$
```

That's fine. Now, you can build a jar with this task:

```
$ clojure -T:build uber
$
```

And the jar will be located at `target` as `target/lib1-0.1-standalone.jar`

That's fine. Now, the problem is that that jar file doesn't print HOLA with the following command

```
$ java -jar target/lib1-0.1-standalone.jar
$
```

What am I doing wrong?

Note: I followed this official document for writing my build.clj file: https://clojure.org/guides/tools_build#_compiled_uberjar_application_build
