## Error posted at:
https://www.eclipse.org/forums/index.php/m/1860602/#msg_1860602

## Followed tutorial:
https://github.com/echebbi/standalone-xtext-example/tree/master

## Other pages solving this differently...

xtext - export dsl as runnable jar:
https://thomas.trocha.com/blog/xtext---export-dsl-as-runnable-jar/

xtext in maven format
https://www.nikostotz.de/blog/combine-xcore-xtend-ecore-and-maven/#generateGenModel.mwe2


xtext Java - export as jar (official documentation)
https://goto40.github.io/self-dsl/xtext_deploy_command_line/
```
...
language = StandardLanguage {
    ...
    generator = {
        generateJavaMain = true
    }
    ...
}
...
```
