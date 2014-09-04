# Steven Snippets for Sublime Text

HTML, CSS and JS snippets for your Sublime Text 2 & 3.

## How to install

### With Package Control

To install through [package control](http://wbond.net/sublime_packages/package_control), search for **Steven Snippets** or typically the keywords **js** or **javascript** are suitable.

### Without Package Control

If you prefer to install it manually, you can download the package and put it inside your `Packages` directory. It should work but will not update automatically.

Go to your Sublime Text 2 Packages directory and clone the repository using the command below:

    git clone git://github.com/wangwen1220/steven-snippets.git steven-snippets

## Console

### [cw] console.warn

```javascript
console.warn(${1:msg});
```

## DOM

### [ae] addEventListener

```javascript
${1:document}.addEventListener('${2:event}', function(e) {
  $3
});
```

### [ac] appendChild

```javascript
${1:document}.appendChild(${2:elem});
```

### [rc] removeChild

```javascript
${1:document}.removeChild(${2:elem});
```

### [ib] insertBefore

```javascript
${1:document}.insertBefore(${2:elem}, ${3:null});
```

### [cel] createElement

```javascript
${1:document}.createElement(${2:elem});
```

### [cdf] createDocumentFragment

```javascript
${1:document}.createDocumentFragment(${2:elem});
```

### [ca] classList.add

```javascript
${1:document}.classList.add('${2:class}');
```

### [ct] classList.toggle

```javascript
${1:document}.classList.toggle('${2:class}');
```

### [cr] classList.remove

```javascript
${1:document}.classList.remove('${2:class}');
```

### [gi] getElementById

```javascript
${1:document}.getElementById('${2:id}');
```

### [gc] getElementsByClassName

```javascript
${1:document}.getElementsByClassName('${2:class}');
```

### [gt] getElementsByTagName

```javascript
${1:document}.getElementsByTagName('${2:tag}');
```

### [ga] getAttribute

```javascript
${1:document}.getAttribute('${2:attr}');
```

### [sa] setAttribute

```javascript
${1:document}.setAttribute('${2:attr}', ${3:value});
```

### [ra] removeAttribute

```javascript
${1:document}.removeAttribute('${2:attr}');
```

### [ih] innerHTML

```javascript
${1:document}.innerHTML = '${2:elem}';
```

### [tc] textContent

```javascript
${1:document}.textContent = '${2:content}';
```

### [qs] querySelector

```javascript
${1:document}.querySelector('${2:selector}');
```

### [qsa] querySelectorAll

```javascript
${1:document}.querySelectorAll('${2:selector}');
```

## Loop

### [fe] forEach

```javascript
${1:myArray}.forEach(function(${2:elem}) {
  ${3}
});
```

### [fi] for in

```javascript
for (${1:prop} in ${2:obj}) {
  if (${2:obj}.hasOwnProperty(${1:prop})) {
    ${3}
  }
}
```

## Function

### [wfn] function

```javascript
function ${1:methodName}(${2:arguments}) {
  ${3}
}
```

### [wafn] anonymous function

```javascript
function(${1:arguments}) {
  ${2}
}
```

### [wii] Immediately-invoked function expression

```javascript
(function($1) {
  $2
})($0);
```

### [wjq] jQuery function

```javascript
(function($) {
  $0
})(jQuery);
```

### [pr] prototype

```javascript
${1:ClassName}.prototype.${2:methodName} = function(${3:arguments}) {
  ${4}
}
```

### [iife] immediately-invoked function expression

```javascript
(function(window, document, undefined) {
  ${1}
})(window, document);
```

### [call] function call

```javascript
${1:methodName}.call(${2:context}, ${3:arguments})
```

### [apply] function apply

```javascript
${1:methodName}.apply(${2:context}, [${3:arguments}])
```

### [ofn] function as a property of an object

```javascript
${1:functionName}: function (${2:arguments}) {
  ${3}
}
```

## Timer

### [si] setInterval

```javascript
setInterval(function() {
  ${2}
}, ${1:delay});
```

### [st] setTimeout

```javascript
setTimeout(function() {
  ${2}
}, ${1:delay});
```

## NodeJS

### [ase] assert.equal

```javascript
assert.equal(${1:actual}, ${2:expected});
```

### [asd] assert.deepEqual

```javascript
assert.deepEqual(${1:actual}, ${2:expected});
```

### [asn] assert.notEqual

```javascript
assert.notEqual(${1:actual}, ${2:expected});
```

### [pe] process.exit

```javascript
process.exit(${1:code});
```

### [pm] prompt

```javascript
prompt(${1:'msg'});
```

## JS Snippets

__do__

```js
do {
  ${1:expression}
} while (${2:condition});
```

__if__

```js
if (${1:condition}) {
  $2
}
```

__ife__

```js
if (${1:condition}) {
  $2
} else {
  $3
}
```

__ifeif__

```js
if (${1:condition}) {
  $2
} else if {
  $3
} else {
  $4
}
```

__for__

```js
for (${1:var i = 0}; ${2:i < ${3:elements.length}}; ${4:i++}) {
  ${5:expression}
}
```

__log__

```js
console.log(${1:'test'});
```

__alt__

```js
alert(${1:'test'});
```

__ls__

```js
if (localStorage.${1:item}) {
  var ${1:item} = localStorage.${1:item};
  $2
}
```

__.pd__

```js
.preventDefault();
```

__.sp__

```js
.stopPropagation();
```

__rand__

```js
Math.floor(Math.random() * ${1:10})
```

__switch__

```js
switch(${1:var}) {
  case $2:
    $3
    break;
  case $4:
    $5
    break;
  default:
    {$6:break};
}
```

__setInterval__

```js
setInterval(function() {
  $2
}, ${1:millis});
```

__setTimeout__

```js
setTimeout(function() {
  $2
}, ${1:millis});
```

__while__

```js
while (${1:condition}) {
  ${2:expression}
};
```

## Author

[Steven Wang](http://wangwen1220.github.io/)