# gulp-csv2json

[![Build Status](https://travis-ci.org/DataGarage/gulp-csv2json.png?branch=master)](https://travis-ci.org/DataGarage/gulp-csv2json)

gulp plugin convert csv to json

## Install

Install with [npm](https://npmjs.org/package/gulp-csv2json)

```
npm install --save-dev gulp-csv2json
```


## Example

```js
var gulp = require('gulp');
var csv2json = require('gulp-csv2json');
var rename = require('gulp-rename');

gulp.task('default', function () {
	gulp.src('src/**/*.csv')
		.pipe(csv2json())
		.pipe(rename({extname: '.json'}))
		.pipe(gulp.dest('dist'));
});
### With delimiter
gulp.task('default', function () {
	gulp.src('src/**/*.csv')
		.pipe(csv2json({delimiter: ';'}))
		.pipe(rename({extname: '.json'}))
		.pipe(gulp.dest('dist'));
});
```


## API

### csv2json(option)
#### options.delimiter
defines the delimiter to be used (default is ',')


## License

MIT [@chilijung](http://github.com/chilijung)
