# <%= projectName %> [![NPM version][npm-image]][npm-url] [![Build Status][travis-image]][travis-url] <%
if (includeCoveralls) { %> [![Coverage percentage][coveralls-image]][coveralls-url]<% } -%>

> <%= description %>

<br>

<% if (!content) { -%>
## Installation

```sh
$ npm install --save <%= projectName %>
```

<br>

## Usage

```js
var <%= safeProjectName %> = require('<%= projectName %>');

<%= safeProjectName %>('Rainbow');
```
<% } else { -%>
<%= content %>
<% } -%>
<br>

## License

<%= license %> © [<%= author.name %>](<%= author.url %>)


[npm-image]: https://badge.fury.io/js/<%= projectName %>.svg
[npm-url]: https://npmjs.org/package/<%= projectName %>
[travis-image]: https://travis-ci.org/<%= githubAccount %>/<%= projectName %>.svg?branch=master
[travis-url]: https://travis-ci.org/<%= githubAccount %>/<%= projectName %>
<% if (includeCoveralls) { -%>
[coveralls-image]: https://coveralls.io/repos/<%= githubAccount %>/<%= projectName %>/badge.svg
[coveralls-url]: https://coveralls.io/r/<%= githubAccount %>/<%= projectName %>
<% } -%>
