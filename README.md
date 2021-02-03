# ngc 9 rc9 rebuild ~6s

```
Angular CLI: 9.0.0-rc.9
Node: 14.15.4
OS: darwin x64

Angular: 9.0.0-rc.9
... animations, cli, common, compiler, compiler-cli, core, forms
... language-service, localize, platform-browser
... platform-browser-dynamic, router
Ivy Workspace: Yes

Package                           Version
-----------------------------------------------------------
@angular-devkit/architect         0.900.0-rc.9
@angular-devkit/build-angular     0.900.0-rc.9
@angular-devkit/build-optimizer   0.900.0-rc.9
@angular-devkit/build-webpack     0.900.0-rc.9
@angular-devkit/core              9.0.0-rc.9
@angular-devkit/schematics        9.0.0-rc.9
@angular/cdk                      9.0.0-rc.8
@angular/material                 9.0.0-rc.8
@ngtools/webpack                  9.0.0-rc.9
@schematics/angular               9.0.0-rc.9
@schematics/update                0.900.0-rc.9
rxjs                              6.5.3
typescript                        3.6.4
webpack                           4.41.2


This triggered rebuilds by appending and removing `console.log(1);` in `projects\one\src\app\a4\a1\a11\a11.component.ts` in `ngOnInit()`

$ ngc -p projects/one/tsconfig.app.json --watch --diagnostics
Time for diagnostics: 19174ms.

Total time: 59s

Compilation complete. Watching for file changes.

File change detected. Starting incremental compilation.

Time for diagnostics: 8104ms.

Total time: 8.2s

Compilation complete. Watching for file changes.

File change detected. Starting incremental compilation.

Time for diagnostics: 5337ms.

Total time: 5.5s

Compilation complete. Watching for file changes.

File change detected. Starting incremental compilation.

Time for diagnostics: 5905ms.

Total time: 6.0s

Compilation complete. Watching for file changes.
```

# NGC 10.2.4 rebuild ~5s
```
Angular CLI: 10.2.1
Node: 14.15.4
OS: darwin x64

Angular: 10.2.4
... animations, common, compiler, compiler-cli, core, forms
... language-service, localize, platform-browser
... platform-browser-dynamic, router
Ivy Workspace: Yes

Package                         Version
---------------------------------------------------------
@angular-devkit/architect       0.1002.1
@angular-devkit/build-angular   0.1002.1
@angular-devkit/core            10.2.1
@angular-devkit/schematics      10.2.1
@angular/cdk                    10.2.7
@angular/cli                    10.2.1
@angular/material               10.2.7
@schematics/angular             10.2.1
@schematics/update              0.1002.1
rxjs                            6.6.3
typescript                      4.0.5


$ ngc -p projects/one/tsconfig.app.json --watch --diagnostics
Time for diagnostics: 21918ms.

Total time: 78s

Compilation complete. Watching for file changes.

File change detected. Starting incremental compilation.

Time for diagnostics: 8601ms.

Total time: 8.9s

Compilation complete. Watching for file changes.

File change detected. Starting incremental compilation.

Time for diagnostics: 8242ms.

Total time: 8.6s

Compilation complete. Watching for file changes.

File change detected. Starting incremental compilation.

Time for diagnostics: 4869ms.

Total time: 5.1s

Compilation complete. Watching for file changes.
```


# ng serve 9rc9 118s

## rebuild 4s -> 3s -> 4s -> 3s -> 3s -> 3s

This is by trigger rebuild by append `console.log(1);` in `projects\one\src\app\a4\a1\a11\a11.component.ts` in `ngOnInit()`
This triggered rebuilds by appending and removing `console.log(1);` in `projects\one\src\app\a4\a1\a11\a11.component.ts` in `ngOnInit()`
```
Date: 2021-02-03T04:14:39.125Z - Hash: 88ae181cad934556acf9 - Time: 118298ms
** Angular Live Development Server is listening on 0.0.0.0:4200, open your browser on http://localhost:4200/ **
: Compiled successfully.

Date: 2021-02-03T04:14:55.800Z - Hash: ef74a87ee7574b111ca8
823 unchanged chunks
chunk {158} 158.de9cf095b3d9dca8a58d.js, 158.de9cf095b3d9dca8a58d.js.map () 15.2 kB  [rendered]
chunk {runtime} runtime.7c820397657aedd64dbf.js, runtime.7c820397657aedd64dbf.js.map (runtime) 32.1 kB [entry] [rendered]
Time: 3675ms
: Compiled successfully.

Date: 2021-02-03T04:15:03.207Z - Hash: 3d98d492920e45ad47b4
823 unchanged chunks
chunk {158} 158.58a34f786ae7ef595f59.js, 158.58a34f786ae7ef595f59.js.map () 15.2 kB  [rendered]
chunk {runtime} runtime.2b595f47367c05f77023.js, runtime.2b595f47367c05f77023.js.map (runtime) 32.1 kB [entry] [rendered]
Time: 3227ms
: Compiled successfully.

Date: 2021-02-03T04:15:10.945Z - Hash: 88ae181cad934556acf9
823 unchanged chunks
chunk {158} 158.95d3556310eab4d654a4.js, 158.95d3556310eab4d654a4.js.map () 15.2 kB  [rendered]
chunk {runtime} runtime.92d12cef4e828ef1b450.js, runtime.92d12cef4e828ef1b450.js.map (runtime) 32.1 kB [entry] [rendered]
Time: 3550ms
: Compiled successfully.

Date: 2021-02-03T04:15:19.378Z - Hash: 3d98d492920e45ad47b4
823 unchanged chunks
chunk {158} 158.58a34f786ae7ef595f59.js, 158.58a34f786ae7ef595f59.js.map () 15.2 kB  [rendered]
chunk {runtime} runtime.2b595f47367c05f77023.js, runtime.2b595f47367c05f77023.js.map (runtime) 32.1 kB [entry] [rendered]
Time: 3105ms
: Compiled successfully.

Date: 2021-02-03T04:15:26.542Z - Hash: ef74a87ee7574b111ca8
823 unchanged chunks
chunk {158} 158.de9cf095b3d9dca8a58d.js, 158.de9cf095b3d9dca8a58d.js.map () 15.2 kB  [rendered]
chunk {runtime} runtime.7c820397657aedd64dbf.js, runtime.7c820397657aedd64dbf.js.map (runtime) 32.1 kB [entry] [rendered]
Time: 3115ms
: Compiled successfully.

Date: 2021-02-03T04:15:34.424Z - Hash: 88ae181cad934556acf9
823 unchanged chunks
chunk {158} 158.95d3556310eab4d654a4.js, 158.95d3556310eab4d654a4.js.map () 15.2 kB  [rendered]
chunk {runtime} runtime.92d12cef4e828ef1b450.js, runtime.92d12cef4e828ef1b450.js.map (runtime) 32.1 kB [entry] [rendered]
Time: 3485ms
: Compiled successfully.
```

# ng serve w/ 10.2.4 149s 

## rebuild -> 5s -> 4s -> 3s -> 3s -> 4s -> 3s

This is by trigger rebuild by append `console.log(1);` in `projects\one\src\app\a4\a1\a11\a11.component.ts` in `ngOnInit()`
```
Date: 2021-02-03T03:56:32.670Z - Hash: 3768479d74e1ab51bb68 - Time: 148893ms

** Angular Live Development Server is listening on 0.0.0.0:4200, open your browser on http://localhost:4200/ **
: Compiled successfully.

Date: 2021-02-03T03:57:46.161Z - Hash: fa836d040e3ea6f910c9
823 unchanged chunks
chunk {158} 158.1a616efe9fe8eb7cd6f8.js, 158.1a616efe9fe8eb7cd6f8.js.map () 14.6 kB  [rendered]
chunk {runtime} runtime.32064e86fb6c6c441e51.js, runtime.32064e86fb6c6c441e51.js.map (runtime) 32.1 kB [entry] [rendered]
Time: 4940ms

: Compiled successfully.

Date: 2021-02-03T03:59:17.392Z - Hash: a60f87ba04d29e5e95a6
823 unchanged chunks
chunk {158} 158.54b2691ab415af8a6306.js, 158.54b2691ab415af8a6306.js.map () 14.6 kB  [rendered]
chunk {runtime} runtime.197796f554a59b24478e.js, runtime.197796f554a59b24478e.js.map (runtime) 32.1 kB [entry] [rendered]
Time: 3883ms
: Compiled successfully.

Date: 2021-02-03T03:59:29.663Z - Hash: f8e4357280fe69277485
823 unchanged chunks
chunk {158} 158.1a616efe9fe8eb7cd6f8.js, 158.1a616efe9fe8eb7cd6f8.js.map () 14.6 kB  [rendered]
chunk {runtime} runtime.32064e86fb6c6c441e51.js, runtime.32064e86fb6c6c441e51.js.map (runtime) 32.1 kB [entry] [rendered]
Time: 3018ms
: Compiled successfully.

Date: 2021-02-03T03:59:36.786Z - Hash: 9e4dc38afdb99afcdbf4
823 unchanged chunks
chunk {158} 158.fafc6a94c1666a0b44a6.js, 158.fafc6a94c1666a0b44a6.js.map () 14.6 kB  [rendered]
chunk {runtime} runtime.fd878e77b138264f8f94.js, runtime.fd878e77b138264f8f94.js.map (runtime) 32.1 kB [entry] [rendered]
Time: 2952ms
: Compiled successfully.


Date: 2021-02-03T04:01:30.695Z - Hash: 9e4dc38afdb99afcdbf4
825 unchanged chunks

Time: 4467ms
: Compiled successfully.

Date: 2021-02-03T04:01:40.772Z - Hash: f8e4357280fe69277485
823 unchanged chunks
chunk {158} 158.1a616efe9fe8eb7cd6f8.js, 158.1a616efe9fe8eb7cd6f8.js.map () 14.6 kB  [rendered]
chunk {runtime} runtime.32064e86fb6c6c441e51.js, runtime.32064e86fb6c6c441e51.js.map (runtime) 32.1 kB [entry] [rendered]
Time: 3196ms
: Compiled successfully.
```
