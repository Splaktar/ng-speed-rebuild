# NGC 9 rc9 rebuild ~5s

```
Angular CLI: 9.0.0-rc.9
Node: 13.6.0
OS: win32 x64

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



> ngc -p projects/one/tsconfig.app.json --watch --diagnostics

Time for diagnostics: 19183ms.

Total time: 73s

Compilation complete. Watching for file changes.

File change detected. Starting incremental compilation.

Time for diagnostics: 6838ms.

Total time: 7.1s

Compilation complete. Watching for file changes.

File change detected. Starting incremental compilation.

Time for diagnostics: 6236ms.

Total time: 6.3s

Compilation complete. Watching for file changes.

File change detected. Starting incremental compilation.

Time for diagnostics: 4907ms.

Total time: 5.0s

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


# ng serve 9rc9 

## rebuild 8s -> 7s -> 5s -> 15s -> 17s -> 14s

This is by trigger rebuild by append `console.log(1);` in `projects\one\src\app\a4\a1\a11\a11.component.ts` in `ngOnInit()`
```
Date: 2020-01-20T14:00:42.768Z - Hash: 876192a2a082a9b27fba - Time: 130468ms
** Angular Live Development Server is listening on 0.0.0.0:4200, open your browser on http://localhost:4200/ **
: Compiled successfully.

Date: 2020-01-20T14:01:38.226Z - Hash: 216d6cd6aee7d37ea96a
823 unchanged chunks
chunk {158} 158.747659e622dc880df2d7.js, 158.747659e622dc880df2d7.js.map () 15.3 kB  [rendered]
chunk {runtime} runtime.aadac18024875aaa5bc4.js, runtime.aadac18024875aaa5bc4.js.map (runtime) 32.1 kB [entry] [rendered]
Time: 8396ms
: Compiled successfully.

Date: 2020-01-20T14:01:53.259Z - Hash: eea13bda59e47b0eff9a
823 unchanged chunks
chunk {158} 158.78c61840dcb5b7251e63.js, 158.78c61840dcb5b7251e63.js.map () 15.3 kB  [rendered]
chunk {runtime} runtime.99149e88ecdfd1b07cd2.js, runtime.99149e88ecdfd1b07cd2.js.map (runtime) 32.1 kB [entry] [rendered]
Time: 6996ms
: Compiled successfully.

Date: 2020-01-20T14:02:03.600Z - Hash: 483086a21f3d0a2bca38
823 unchanged chunks
chunk {158} 158.b3e751cc9ccb1ffe8699.js, 158.b3e751cc9ccb1ffe8699.js.map () 15.3 kB  [rendered]
chunk {runtime} runtime.8da87e3dfa50df71ac40.js, runtime.8da87e3dfa50df71ac40.js.map (runtime) 32.1 kB [entry] [rendered]
Time: 5252ms
: Compiled successfully.

Date: 2020-01-20T14:02:30.355Z - Hash: 37f76ffb90983a9ffe01
823 unchanged chunks
chunk {158} 158.517f4809cb42f2300f7a.js, 158.517f4809cb42f2300f7a.js.map () 15.3 kB  [rendered]
chunk {runtime} runtime.f99fbe2cb3f1a38514e8.js, runtime.f99fbe2cb3f1a38514e8.js.map (runtime) 32.1 kB [entry] [rendered]
Time: 15432ms
: Compiled successfully.

Date: 2020-01-20T14:04:33.933Z - Hash: 22b5fb25ebd6c153e885
823 unchanged chunks
chunk {158} 158.19cce3587bac1b7613fd.js, 158.19cce3587bac1b7613fd.js.map () 15.4 kB  [rendered]
chunk {runtime} runtime.697285100ffce366990e.js, runtime.697285100ffce366990e.js.map (runtime) 32.1 kB [entry] [rendered]
Time: 17722ms
: Compiled successfully.

Date: 2020-01-20T14:04:56.453Z - Hash: 753c04175437c21b1948
823 unchanged chunks
chunk {158} 158.4203179597cc67ea241b.js, 158.4203179597cc67ea241b.js.map () 15.4 kB  [rendered]
chunk {runtime} runtime.6980764238e10f1063f0.js, runtime.6980764238e10f1063f0.js.map (runtime) 32.1 kB [entry] [rendered]
Time: 14322ms
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
