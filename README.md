grunt-include-replace [![Dependency Status](http://david-dm.org/alanshaw/grunt-include-replace.png)](http://david-dm.org/alanshaw/grunt-include-replace)
=====================

_Unreleased_ Grunt task to include files and replace variables.

Will allow parameterised file includes:
 
hello.html

```html
<!DOCTYPE html>
<h1>Hello World!</h1>
<p>@@include('/path/to/include/message.html', {"name": "Joe Bloggs"})</p>
```

message.html

```html
Hello @@name!
```

Result:

```html
<!DOCTYPE html>
<h1>Hello World!</h1>
<p>Hello Joe Bloggs!</p>
```

WARNING: The task _does not_ check for recursive includes.