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
+ gulp@4.0.2 (For licensing)
+ gulp-append-prepend@1.0.8 (For licensing)
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
