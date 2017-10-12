```
[~/src/tools.decompiler-aot]> unzip tools.decompiler.jar -d classes
... output elided ...
[~/src/tools.decompiler-aot]> clj
Clojure 1.9.0-beta2
user=> (use 'clojure.tools.decompiler)
nil
user=> (decompile-classfiles {:input-path "classes" :output-path "src"})
Decompiling classes/clojure/tools/decompiler__init.class to src/clojure/tools/decompiler.clj
Decompiling classes/clojure/tools/decompiler/sugar__init.class to src/clojure/tools/decompiler/sugar.clj
Decompiling classes/clojure/tools/decompiler/compact__init.class to src/clojure/tools/decompiler/compact.clj
Decompiling classes/clojure/tools/decompiler/bc__init.class to src/clojure/tools/decompiler/bc.clj
Decompiling classes/clojure/tools/decompiler/pprint__init.class to src/clojure/tools/decompiler/pprint.clj
Decompiling classes/clojure/tools/decompiler/source__init.class to src/clojure/tools/decompiler/source.clj
Decompiling classes/clojure/tools/decompiler/ast__init.class to src/clojure/tools/decompiler/ast.clj
Decompiling classes/clojure/tools/decompiler/utils__init.class to src/clojure/tools/decompiler/utils.clj
nil
user=>
[~/src/tools.decompiler-aot]> tree src
src
└── clojure
    └── tools
        ├── decompiler
        │   ├── ast.clj
        │   ├── bc.clj
        │   ├── compact.clj
        │   ├── pprint.clj
        │   ├── source.clj
        │   ├── sugar.clj
        │   └── utils.clj
        └── decompiler.clj

3 directories, 8 files
```
