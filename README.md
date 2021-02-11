# An_overview_of_Gulp-js.
# GulpJS
<p align="center">
  <a href="https://gulpjs.com">
    <img height="257" width="114" src="https://raw.githubusercontent.com/gulpjs/artwork/master/gulp-2x.png">
  </a>
  <p align="center">The streaming build system</p>
</p> 

About 2 months ago I discovered gulpjs. It was a fantastic tool for frontend developers. Especially when I wrote sass codes, I was wasting time on compiling.I need to compress  js, css and images files for using good seo in my website. In that situation I used some website for compress my web code files. However  I realized that Gulp can made it for my project. It was useful




## What is gulp?

- **Automation** - gulp is a toolkit that helps you automate painful or time-consuming tasks in your development workflow.
- **Platform-agnostic** - Integrations are built into all major IDEs and people are using gulp with PHP, .NET, Node.js, Java, and other platforms.
- **Strong Ecosystem** - Use npm modules to do anything you want + over 3000 curated plugins for streaming file transformations.
- **Simple** - By providing only a minimal API surface, gulp is easy to learn and simple to use.


## Installation
Install Gulp....
```bash
npm install gulp-cli -g
npm install gulp -D

```
After that we should create packed.json file. Copy adn Paste it your packet.json file

 
```bash
 {
  "name": "frontend",
  "version": "1.0.0",
  "main": "gulpfile.js",
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1"
  },
  "keywords": [],
  "author": "",
  "license": "ISC",
  "description": "",
  "dependencies": {},
  "devDependencies": {
    "browser-sync": "^2.26.3",
    "del": "^3.0.0",
    "gulp": "^3.9.1",
    "gulp-autoprefixer": "^6.0.0",
    "gulp-concat": "^2.6.1",
    "gulp-csso": "^3.0.1",
    "gulp-htmlmin": "^5.0.1",
    "gulp-imagemin": "^4.1.0",
    "gulp-sass": "^4.0.2",
    "gulp-uglify": "^3.0.1",
    "run-sequence": "^2.2.1"
  }
}

```
We need to gulpfile.js. Especially that file must be  name  is gulpfile.js. We should copy and paste it your gulpfile.js file.
```
const gulp = require('gulp');
const browserSync = require('browser-sync').create();
const sass = require('gulp-sass');
const minifyCSS = require('gulp-csso');
const minifyImg = require('gulp-imagemin');
const minifyJS = require('gulp-uglify');
const minifyHTML = require('gulp-htmlmin');
const concat = require('gulp-concat');
const autoprefixer = require('gulp-autoprefixer');
const del = require('del');
const runSequence = require('run-sequence');
```

Now we can create tasks and do our operations.

```
gulp.task('task_adi', () => {
    // Operations
});

```
## GulpJs Tutorial





 
## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.
