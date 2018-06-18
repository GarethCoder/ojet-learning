# Ojet Learing

### OJET BIND IF

- ``ojet-bind-if`` to conditionally render its contents only if a provided
test returns true.

#### Example

``` 
<oj-bind-if test="[[myTest]]">
	<div>My Contents</div>
</oj-bind-if>

```

### OJET BIND FOR EACH

- Use ``<oj-bind-for-each>`` to bind items of an array to the specified markup section. 
The markup section is duplicated for each array item when element is rendered. 
- ``<oj-bind-for-each>`` requires the application to specify a single ``<template>`` element as its direct child. The markup being stamped out should be placed 
inside of this <template> element.

#### Example

```
<oj-bind-for-each data='[{"type":"Apple"},{"type":"Orange"}]'>
 <template>
	<p><oj-bind-text value='[[$current.data.type]]'></oj-bind-text></p>
</template>
</oj-bind-for-each>

```

### OJET BIND TEXT

- Use ``<oj-bind-text>`` to bind a text node to a variable.

#### Example

```
<span>
 <oj-bind-text value='[[myText]]'></oj-bind-text>
</span>

```
