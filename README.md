# gulp-csv2json

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

gulp.task('default', function () {
	gulp.src('src/**/*.csv')
		.pipe(csv2json())
		.pipe(gulp.dest('dist'));
});
```


## API

### csv2json()


## License

MIT [@chilijung](http://github.com/chilijung)