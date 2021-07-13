## [1.2.1] 2021-07-13

### Bug fixing

### Major style changes

### Deleted components

### Added components

### Deleted dependencies

### Added dependencies

### Updated dependencies

```
@fortawesome/fontawesome-free    5.15.2   →    5.15.3
  @fullcalendar/core                5.5.1   →     5.8.0
  @fullcalendar/daygrid             5.5.0   →     5.8.0
  @fullcalendar/interaction         5.5.0   →     5.8.0
  classnames                        2.2.6   →     2.3.1
  dropzone                          5.7.2   →     5.9.2
  node-sass                        4.14.1   →     6.0.1
  nouislider                       14.6.3   →    15.2.0
  react                            17.0.1   →    17.0.2
  react-dom                        17.0.1   →    17.0.2
  react-scripts                     4.0.1   →     4.0.3
  react-to-print                   2.12.2   →    2.12.6
  sweetalert2                     10.13.0   →   11.0.18
  eslint-plugin-flowtype            5.2.0   →     5.8.0
  gulp-append-prepend               1.0.8   →     1.0.9
  typescript                        4.1.3   →     4.3.5
```

### Warning

**The TypeScript dependencies are installed only to stop console warnings on install. They are not actually used in our product. So the product is not on TypeScript!**
_The following warnings will appear when running the installation command, but they do not affect the UI or the functionality of the product (they will be solved in our next update):_

```
npm WARN react-bootstrap-table-next@4.0.3 requires a peer of react@^16.3.0 but none is installed. You must install peer dependencies yourself.
npm WARN react-bootstrap-table-next@4.0.3 requires a peer of react-dom@^16.3.0 but none is installed. You must install peer dependencies yourself.
npm WARN react-bootstrap-table2-paginator@2.1.2 requires a peer of react@^16.3.0 but none is installed. You must install peer dependencies yourself.
npm WARN react-bootstrap-table2-paginator@2.1.2 requires a peer of react-dom@^16.3.0 but none is installed. You must install peer dependencies yourself.
npm WARN react-bootstrap-table2-toolkit@2.1.3 requires a peer of react@^16.3.0 but none is installed. You must install peer dependencies yourself.
npm WARN react-bootstrap-table2-toolkit@2.1.3 requires a peer of react-dom@^16.3.0 but none is installed. You must install peer dependencies yourself.
npm WARN react-quill@1.3.5 requires a peer of react@^0.14.9 || ^15.3.0 || ^16.0.0 but none is installed. You must install peer dependencies yourself.
npm WARN react-datetime@3.0.4 requires a peer of react@^16.5.0 but none is installed. You must install peer dependencies yourself.
npm WARN react-select2-wrapper@1.0.4-beta6 requires a peer of react@^0.14.0 || ^15.0.0-rc || ^15.0.0 || ^16.0.0 but none is installed. You must install peer dependencies yourself.
npm WARN react-select2-wrapper@1.0.4-beta6 requires a peer of react-dom@^0.14.0 || ^15.0.0-rc || ^15.0.0 || ^16.0.0 but none is installed. You must install peer dependencies yourself.
npm WARN @babel/plugin-bugfix-v8-spread-parameters-in-optional-chaining@7.14.5 requires a peer of @babel/core@^7.13.0 but none is installed. You must install peer dependencies yourself.
```

_If they will persist in our 2.*.* version, we will drop their usages and replace them with other plugins._
_In development mode, some of the above plugins will throw a warning because they still use React v16 syntax. If the error will persist in our 2.*.* version, we will drop their usage and replace them with other plugins._

**Note:** There are 11 vulnerabilities when running the `npm install` command, to fix it just run the following command `npm audit fix` once the installation is finished.

## [1.2.0] 2021-01-25

### Bug fixing

- https://github.com/creativetimofficial/ct-argon-dashboard-pro-react/issues/26
- https://github.xcom/creativetimofficial/ct-argon-dashboard-pro-react/issues/21 (this was auto solved by the new reactstrap version)
- https://github.com/creativetimofficial/ct-argon-dashboard-pro-react/issues/19
- https://github.com/creativetimofficial/ct-argon-dashboard-pro-react/issues/17

### Major style changes

- Delete the `src/assets/scss/bootstrap` folder and changed all the bootstrap imports from `src/assets/scss` files to ones from `node_modules`

### Deleted components

### Added components

### Deleted dependencies

- react-google-maps (We'll use the Google Maps API with Vanilla JS instead)
- @types/googlemaps (since the deletion of the react-google-maps)
- @types/markerclustererplus (since the deletion of the react-google-maps)
- @types/react (since the deletion of the react-google-maps)
- react-tagsinput (since it is no longer maintained - we've created our own component based on this one, so you will have all the functionality from it)

### Added dependencies

- sweetalert2@10.13.0 (so that we can import the styles from node_modules, not a downloaded version)
- select2@4.0.13 (so that we can import the styles from node_modules, not a downloaded version)
- @fortawesome/fontawesome-free@5.15.2 (so that we can import the styles from node_modules, not a downloaded version)
- quill@1.3.7 (so that we can import the styles from node_modules, not a downloaded version)
- bootstrap@4.6.0 (and deleted the downloaded version of Bootstrap)
- node-sass-package-importer@5.3.2 (so we can import bootstrap from node_modules)

### Updated dependencies

```
@fullcalendar/core                   4.4.0   →    5.5.1
@fullcalendar/daygrid                4.4.0   →    5.5.0
@fullcalendar/interaction            4.4.0   →    5.5.0
chart.js                             2.9.3   →    2.9.4
dropzone                             5.7.0   →    5.7.2
list.js                              1.5.0   →    2.3.1
moment                              2.24.0   →   2.29.1
node-sass                           4.13.1   →   4.14.1
nouislider                          14.1.1   →   14.6.3
react                              16.12.0   →   17.0.1
react-bootstrap-sweetalert           5.1.9   →    5.2.0
react-bootstrap-table-next           3.3.5   →    4.0.3
react-bootstrap-table2-paginator     2.1.0   →    2.1.2
react-bootstrap-table2-toolkit       2.1.2   →    2.1.3
react-chartjs-2                      2.9.0   →   2.11.1
react-copy-to-clipboard              5.0.2   →    5.0.3
react-datetime                      2.16.3   →    3.0.4
react-dom                          16.12.0   →   17.0.1
react-jvectormap                    0.0.15   →   0.0.16
react-notification-alert            0.0.12   →   0.0.13
react-quill                          1.3.3   →    1.3.5
react-router                         5.1.2   →    5.2.0
react-router-dom                     5.1.2   →    5.2.0
react-scripts                        3.4.0   →    4.0.1
react-to-print                       2.5.1   →   2.12.2
reactstrap                           8.4.1   →    8.9.0
eslint-plugin-flowtype              3.13.0   →    5.2.0
typescript                           3.7.5   →    4.1.3
```

### Warning

**The TypeScript dependencies are installed only to stop console warnings on install. They are not actually used in our product. So the product is not on TypeScript!**
_The following warnings will appear when running the installation command, but they do not affect the UI or the functionality of the product (they will be solved in our next update):_

```
npm WARN react-bootstrap-table2-paginator@2.1.2 requires a peer of react@^16.3.0 but none is installed. You must install peer dependencies yourself.
npm WARN react-bootstrap-table2-paginator@2.1.2 requires a peer of react-dom@^16.3.0 but none is installed. You must install peer dependencies yourself.
npm WARN react-bootstrap-table-next@4.0.3 requires a peer of react@^16.3.0 but none is installed. You must install peer dependencies yourself.
npm WARN react-bootstrap-table-next@4.0.3 requires a peer of react-dom@^16.3.0 but none is installed. You must install peer dependencies yourself.
npm WARN react-bootstrap-table2-toolkit@2.1.3 requires a peer of react@^16.3.0 but none is installed. You must install peer dependencies yourself.
npm WARN react-bootstrap-table2-toolkit@2.1.3 requires a peer of react-dom@^16.3.0 but none is installed. You must install peer dependencies yourself.
npm WARN react-datetime@3.0.4 requires a peer of react@^16.5.0 but none is installed. You must install peer dependencies yourself.
npm WARN react-quill@1.3.5 requires a peer of react@^0.14.9 || ^15.3.0 || ^16.0.0 but none is installed. You must install peer dependencies yourself.
npm WARN react-select2-wrapper@1.0.4-beta6 requires a peer of react@^0.14.0 || ^15.0.0-rc || ^15.0.0 || ^16.0.0 but none is installed. You must install peer dependencies yourself.
npm WARN react-select2-wrapper@1.0.4-beta6 requires a peer of react-dom@^0.14.0 || ^15.0.0-rc || ^15.0.0 || ^16.0.0 but none is installed. You must install peer dependencies yourself.
npm WARN react-popper@1.3.7 requires a peer of react@0.14.x || ^15.0.0 || ^16.0.0 but none is installed. You must install peer dependencies yourself.
npm WARN create-react-context@0.3.0 requires a peer of react@^0.14.0 || ^15.0.0 || ^16.0.0 but none is installed. You must install peer dependencies yourself.
```

_If they will persist in our 2.*.* version, we will drop their usages and replace them with other plugins._
_In development mode, some of the above plugins will throw a warning because they still use React v16 syntax. If the error will persist in our 2.*.* version, we will drop their usage and replace them with other plugins._

## [1.1.0] 2020-02-21

### Bug fixing

- Change the usage of `componentWillMount` to the usage of `constructor`
- Move `maxBarThickness` inside charts variables from the global initialization
- Add `scrollTop` on `componentDidMount` for `Auth` layout
- Github:
  - https://github.com/creativetimofficial/ct-argon-dashboard-pro-react/issues/15
  - https://github.com/creativetimofficial/ct-argon-dashboard-pro-react/issues/14
  - https://github.com/creativetimofficial/ct-argon-dashboard-pro-react/issues/13
  - https://github.com/creativetimofficial/ct-argon-dashboard-pro-react/issues/8
  - https://github.com/creativetimofficial/ct-argon-dashboard-pro-react/issues/6
  - https://github.com/creativetimofficial/ct-argon-dashboard-pro-react/issues/2

### Major style changes

- Changed almost all files from the scss folder (`src/assets/scss/*`)

### Deleted components

### Added components

- Added page and layout for RTL Support

### Deleted dependencies

### Added dependencies

- gulp@4.0.2 (For licensing)
- gulp-append-prepend@1.0.8 (For licensing)

### Updated dependencies

```
@fullcalendar/core                   4.0.2   →     4.4.0
@fullcalendar/daygrid                4.0.1   →     4.4.0
@fullcalendar/interaction            4.0.2   →     4.4.0
chart.js                             2.8.0   →     2.9.3
dropzone                             5.5.1   →     5.7.0
node-sass                           4.11.0   →    4.13.1
nouislider                          13.1.4   →    14.1.1
react                               16.8.6   →   16.12.0
react-bootstrap-sweetalert           4.4.1   →     5.1.9
react-bootstrap-table-next           3.1.0   →     3.3.5
react-bootstrap-table2-paginator     2.0.5   →     2.1.0
react-bootstrap-table2-toolkit       1.4.0   →     2.1.2
react-chartjs-2                      2.7.6   →     2.9.0
react-copy-to-clipboard              5.0.1   →     5.0.2
react-dom                           16.8.6   →   16.12.0
react-jvectormap                     0.0.6   →    0.0.15
react-perfect-scrollbar              1.4.4   →     1.5.8
react-router                         5.0.0   →     5.1.2
react-router-dom                     5.0.0   →     5.1.2
react-scripts                        2.1.8   →     3.4.0
react-to-print                       2.1.0   →     2.5.1
reactstrap                           8.0.0   →     8.4.1
@types/googlemaps                  3.30.19   →    3.39.2
@types/react                       16.8.13   →   16.9.21
typescript                           3.4.3   →     3.7.5
```

### Warning

**The following warnings could not be solved, due to some of our dependencies, however, they do not affect the functionality or the UI of the product:**

```
npm WARN deprecated request@2.88.2: request has been deprecated, see https://github.com/request/request/issues/3142
npm WARN deprecated core-js@2.6.11: core-js@<3 is no longer maintained and not recommended for usage due to the number of issues. Please, upgrade your dependencies to the actual version of core-js@3.
npm WARN deprecated popper.js@1.16.1: Popper changed home, find its new releases at @popperjs/core
```

**The following warning could not be solved due to the usage of react-google-maps and react-jvectormap (Note: if the warning will persist after React changes version to 17, we'll drop the support for react-google-maps and react-jvectormap, and replace them with other react library for maps):**

```
Warning: componentWillMount has been renamed, and is not recommended for use. See https://fb.me/react-unsafe-component-lifecycles for details.

* Move code with side effects to componentDidMount, and set initial state in the constructor.
* Rename componentWillMount to UNSAFE_componentWillMount to suppress this warning in non-strict mode. In React 17.x, only the UNSAFE_ name will work. To rename all deprecated lifecycles to their new names, you can run `npx react-codemod rename-unsafe-lifecycles` in your project source folder.

Please update the following components: e
```

**The following warning could not be solved due to the usage of DateTime, Quill, Select2, TagsInput (Note: if the warning will persist after React changes version to 17, we'll drop the support for DateTime, Quill, Select2, TagsInput, and replace them with other libraries for date pickers, live editors, selects and tags inputs):**

```
react-dom.development.js:12357 Warning: componentWillReceiveProps has been renamed, and is not recommended for use. See https://fb.me/react-unsafe-component-lifecycles for details.

* Move data fetching code or side effects to componentDidUpdate.
* If you're updating state whenever props change, refactor your code to use memoization techniques or move it to static getDerivedStateFromProps. Learn more at: https://fb.me/react-derived-state
* Rename componentWillReceiveProps to UNSAFE_componentWillReceiveProps to suppress this warning in non-strict mode. In React 17.x, only the UNSAFE_ name will work. To rename all deprecated lifecycles to their new names, you can run `npx react-codemod rename-unsafe-lifecycles` in your project source folder.

Please update the following components: DateTime, Quill, Select2, TagsInput
```

```
react-dom.development.js:12357 Warning: componentWillUpdate has been renamed, and is not recommended for use. See https://fb.me/react-unsafe-component-lifecycles for details.

* Move data fetching code or side effects to componentDidUpdate.
* Rename componentWillUpdate to UNSAFE_componentWillUpdate to suppress this warning in non-strict mode. In React 17.x, only the UNSAFE_ name will work. To rename all deprecated lifecycles to their new names, you can run `npx react-codemod rename-unsafe-lifecycles` in your project source folder.

Please update the following components: Quill
```

## [1.0.0] 2019-04-10

### Original Release

- Added Reactstrap as base framework
- Added design from Argon Dashboard PRO by Creative Tim
