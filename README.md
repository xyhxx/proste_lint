# proste_lint
> You can view <a href="https://dart-lang.github.io/linter/lints/">all the rules</a>, select the rules that suit your project and adjust the rules in the file

1. add package in dev_dependencies

```
dev_dependencies:
  proste_lint: last
```

2. create a `analysis_options.yaml` in root directory

3. include proste_list

``` yaml
include: package:proste_lint/analysis_options.yaml
```

4. if you want off some rules or add some rules

``` yaml
include: package:proste_lint/analysis_options.yaml
# add new wanning tips
analyzer:
  errors:
    avoid_annotating_with_dynamic: warning # info, warning, error

linter:
  rules: 
    prefer_expression_function_bodies: false # off
    avoid_annotating_with_dynamic: true # on


```


```

MIT License

Copyright (c) 2021 xyhxx

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

```
