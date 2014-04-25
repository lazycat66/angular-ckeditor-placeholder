# angular-ckeditor-placeholder

[![Build Status](https://travis-ci.org/lemonde/angular-ckeditor-placeholder.svg?branch=master)](https://travis-ci.org/lemonde/angular-ckeditor-placeholder)
[![Dependency Status](https://david-dm.org/lemonde/angular-ckeditor-placeholder.svg?theme=shields.io)](https://david-dm.org/lemonde/angular-ckeditor-placeholder)
[![devDependency Status](https://david-dm.org/lemonde/angular-ckeditor-placeholder/dev-status.svg?theme=shields.io)](https://david-dm.org/lemonde/angular-ckeditor-placeholder#info=devDependencies)

Placeholder support for CKEditor angular directive.

## Install

### Using bower

```sh
bower install angular-ckeditor-placeholder
```

## Usage

HTML:

```html
<!-- Load files. -->
<script src="angular.js"></script>
<script src="angular-ckeditor.js"></script>
<script src="angular-ckeditor-placeholder.js"></script>

<div ng-controller="CkeditorCtrl">
  <div ckeditor="options" ng-model="title" placeholder="Title"></div>
</div>
```

JavaScript:

```js
angular.module('controllers.ckeditor', ['ckeditor'])
.controller('CkeditorCtrl', function ($scope) {

  // Editor options.
  $scope.options = {
    language: 'en',
    allowedContent: true,
    entities: false
  };
});
```

## License

MIT