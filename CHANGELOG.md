## [Unreleased]

### Changed
- Create build script for GitHub pages with GitHub actions to allow for custom building
  [#1203](https://github.com/nextcloud/cookbook/pull/1203) @christianlupus

### Fixed
- Added new public page styling in preparation for NC25
  [#1201](https://github.com/nextcloud/cookbook/pull/1201) @christianlupus
- Fix API endpoint helpers to enforce JSON answers and minor styling enhancements
  [#1202](https://github.com/nextcloud/cookbook/pull/1202) @christianlupus
- Fix XPath to allow for microdata parsing with multiple adjacent schema objects in HTML code
  [#1220](https://github.com/nextcloud/cookbook/pull/1220) @christianlupus
- Fix filters for array-valued entries in recipes
  [#1222](https://github.com/nextcloud/cookbook/pull/1222) @christianlupus

### Maintenance
- Use the pre-built database images for MySQL and PostgreSQL tests
  [#1204](https://github.com/nextcloud/cookbook/pull/1204) @christianlupus
- Update stylelint-config-idiomatic and fix code styling
  [#1224](https://github.com/nextcloud/cookbook/pull/1224) @christianlupus
- Remove obsolete code from Recipe service class
  [#1226](https://github.com/nextcloud/cookbook/pull/1226) @christianlupus
- Allow for PlantUML diagrams in documentation
  [#1229](https://github.com/nextcloud/cookbook/pull/1229) @christianlupus

### Removed
- Remove the deprecated endpoints from version 0.9.15
  [#1200](https://github.com/nextcloud/cookbook/pull/1200) @christianlupus


## 0.9.15 - 2022-09-08

### Added
- Create structure to run integration tests against a real database
  [#1195](https://github.com/nextcloud/cookbook/pull/1195) @christianlupus

### Changed
- Migrate ILogger to LoggerInterface
  [#1192](https://github.com/nextcloud/cookbook/pull/1192) @miles170

### Fixed
- Close security issue by enabling CSRF protection on most endpoints
  [#1190](https://github.com/nextcloud/cookbook/pull/1190) @christianlupus
- Fix bug in DB access class to prevent PostgreSQL from viewing all recipes of a category
  [#1195](https://github.com/nextcloud/cookbook/pull/1195) @christianlupus
- Fix minor bug to make API access consistent with API definitions and internal structure more well-defined
  [#1195](https://github.com/nextcloud/cookbook/pull/1195) @christianlupus

### Documentation
- Defining new API interface to fix security issue
  [#1186](https://github.com/nextcloud/cookbook/pull/1186) @christianlupus
- Fixed API description w.r.t. return types and examples 
  (see [#1153](https://github.com/nextcloud/cookbook/issues/1153)) @christianlupus

### Deprecated
- Deprecate NC core version V21
  [#1195](https://github.com/nextcloud/cookbook/pull/1195) @christianlupus

### Removed
- Removed support for NC core <= V20
  [#1195](https://github.com/nextcloud/cookbook/pull/1195) @christianlupus


## 0.9.14 - 2022-08-29

### Changed
- Parsing of JSON recipe objects in a cascade of filters
  [#1097](https://github.com/nextcloud/cookbook/pull/1097) @christianlupus
- Ordering corrected for mobile and printout versions
  [#1107](https://github.com/nextcloud/cookbook/pull/1107) @christianlupus
- Less intrusive sharp popup (suggestion menu for reference autocomplete)
  [#1098](https://github.com/nextcloud/cookbook/pull/1098) @MarcelRobitaille

### Fixed
- Prevent slow loading of recipes due to iteration over all files
  [#1072](https://github.com/nextcloud/cookbook/pull/1072) @christianlupus
- Fix keyword ordering buttons being clipped by top bar
  [#1103](https://github.com/nextcloud/cookbook/pull/1103) @MarcelRobitaille
- Replace print icon with something better recognizable
  [#1106](https://github.com/nextcloud/cookbook/pull/1106) @christianlupus
- Make recipeYield optional
  [#1108](https://github.com/nextcloud/cookbook/pull/1108) @christianlupus
- Fix UI glitches caused by improper use of Breadcrumbs component
  [#1105](https://github.com/nextcloud/cookbook/pull/1105) @MarcelRobitaille
- Fix typos and styling issues
  [#1112](https://github.com/nextcloud/cookbook/pull/1112) @christianlupus
- Fix API endpoint used for updating recipes
  [#1119](https://github.com/nextcloud/cookbook/pull/1119) @MarcelRobitaille
- Reactivate step debugging  in PHP
  [#1160](https://github.com/nextcloud/cookbook/pull/1160) @christianlupus
- Fix multi-line code entry in some fields during editing
  [#1162](https://github.com/nextcloud/cookbook/pull/1162) @christianlupus
- Make the API return correct nutrition information objects for recipes
  [#1163](https://github.com/nextcloud/cookbook/pull/1163) @christianlupus
- Allow HowToSteps in recipe instructions during importing
  [#1165](https://github.com/nextcloud/cookbook/pull/1165) @christianlupus
- Correct output of getApiVersion
  [#1175](https://github.com/nextcloud/cookbook/pull/1175) @christianlupus

### Maintenance
- Add composer.json to version control to have unique installed dependency versions
  [#1093](https://github.com/nextcloud/cookbook/pull/1093) @christianlupus
- Update supported PHP versions
  [#1095](https://github.com/nextcloud/cookbook/pull/1095) @christianlupus
- Update README with app screenshot and fixed repository links
  [#1102](https://github.com/nextcloud/cookbook/pull/1102) @MarcelRobitaille
- Cleaned up entry JS code
  [#1118](https://github.com/nextcloud/cookbook/pull/1118) @christianlupus
- Create Python based testing wrapper and enhance workflow script
  [#1137](https://github.com/nextcloud/cookbook/pull/1137) @christianlupus
- Update workflow from nextcloud organization template
  [#1142](https://github.com/nextcloud/cookbook/pull/1142) @christianlupus
- Remove dependency @nextcloud/auth from explicit dependencies
  [#1149](https://github.com/nextcloud/cookbook/pull/1149) @christianlupus
- Fix bug in automated test programs
  [#1165](https://github.com/nextcloud/cookbook/pull/1165) @christianlupus
- Update some NPM dependencies and deprecations
  [#1159](https://github.com/nextcloud/cookbook/pull/1159) @christianlupus
- Prepare the generation of pre-releases
  [#1169](https://github.com/nextcloud/cookbook/pull/1169) @christianlupus
- Corrected usage of npm ci
  [#1170](https://github.com/nextcloud/cookbook/pull/1170) @christianlupus
- Reactivate Codecov coverage reporting
  [#1177](https://github.com/nextcloud/cookbook/pull/1177) @christianlupus


## 0.9.14-beta2 - 2022-08-24

### Fixed
- Correct output of getApiVersion
  [#1175](https://github.com/nextcloud/cookbook/pull/1175) @christianlupus


## 0.9.14-beta1 - 2022-08-23

### Changed
- Parsing of JSON recipe objects in a cascade of filters
  [#1097](https://github.com/nextcloud/cookbook/pull/1097) @christianlupus
- Ordering corrected for mobile and printout versions
  [#1107](https://github.com/nextcloud/cookbook/pull/1107) @christianlupus
- Less intrusive sharp popup (suggestion menu for reference autocomplete)
  [#1098](https://github.com/nextcloud/cookbook/pull/1098) @MarcelRobitaille

### Fixed
- Prevent slow loading of recipes due to iteration over all files
  [#1072](https://github.com/nextcloud/cookbook/pull/1072) @christianlupus
- Fix keyword ordering buttons being clipped by top bar
  [#1103](https://github.com/nextcloud/cookbook/pull/1103) @MarcelRobitaille
- Replace print icon with something better recognizable
  [#1106](https://github.com/nextcloud/cookbook/pull/1106) @christianlupus
- Make recipeYield optional
  [#1108](https://github.com/nextcloud/cookbook/pull/1108) @christianlupus
- Fix UI glitches caused by improper use of Breadcrumbs component
  [#1105](https://github.com/nextcloud/cookbook/pull/1105) @MarcelRobitaille
- Fix typos and styling issues
  [#1112](https://github.com/nextcloud/cookbook/pull/1112) @christianlupus
- Fix API endpoint used for updating recipes
  [#1119](https://github.com/nextcloud/cookbook/pull/1119) @MarcelRobitaille
- Reactivate step debugging  in PHP
  [#1160](https://github.com/nextcloud/cookbook/pull/1160) @christianlupus
- Fix multi-line code entry in some fields during editing
  [#1162](https://github.com/nextcloud/cookbook/pull/1162) @christianlupus
- Make the API return correct nutrition information objects for recipes
  [#1163](https://github.com/nextcloud/cookbook/pull/1163) @christianlupus
- Allow HowToSteps in recipe instructions during importing
  [#1165](https://github.com/nextcloud/cookbook/pull/1165) @christianlupus

### Maintenance
- Add composer.json to version control to have unique installed dependency versions
  [#1093](https://github.com/nextcloud/cookbook/pull/1093) @christianlupus
- Update supported PHP versions
  [#1095](https://github.com/nextcloud/cookbook/pull/1095) @christianlupus
- Update README with app screenshot and fixed repository links
  [#1102](https://github.com/nextcloud/cookbook/pull/1102) @MarcelRobitaille
- Cleaned up entry JS code
  [#1118](https://github.com/nextcloud/cookbook/pull/1118) @christianlupus
- Create Python based testing wrapper and enhance workflow script
  [#1137](https://github.com/nextcloud/cookbook/pull/1137) @christianlupus
- Update workflow from nextcloud organization template
  [#1142](https://github.com/nextcloud/cookbook/pull/1142) @christianlupus
- Remove dependency @nextcloud/auth from explicit dependencies
  [#1149](https://github.com/nextcloud/cookbook/pull/1149) @christianlupus
- Fix bug in automated test programs
  [#1165](https://github.com/nextcloud/cookbook/pull/1165) @christianlupus
- Update some NPM dependencies and deprecations
  [#1159](https://github.com/nextcloud/cookbook/pull/1159) @christianlupus
- Prepare the generation of pre-releases
  [#1169](https://github.com/nextcloud/cookbook/pull/1169) @christianlupus
- Corrected usage of npm ci
  [#1170](https://github.com/nextcloud/cookbook/pull/1170) @christianlupus


## 0.9.13 - 2022-07-02

### Added
- Create service class for downloading and extracting JSON
  [#553](https://github.com/nextcloud/cookbook/pull/553) @christianlupus
- Show recipe titles for internal references
  [#1063](https://github.com/nextcloud/cookbook/pull/1063) @christianlupus

### Changed
- Extracted user folder handling into its own helper class
  [#1007](https://github.com/nextcloud/cookbook/pull/1007) @christianlupus
- Switched to cURL for downloading of external files
  [#1055](https://github.com/nextcloud/cookbook/pull/1055) @christianlupus
- Rewrite encoding of imported recipes
  [#1057](https://github.com/nextcloud/cookbook/pull/1057) @christianlupus
  
### Fixed
- Fix visual regression in edit mode to prevent overflow of breadcrumbs
  [#989](https://github.com/nextcloud/cookbook/pull/989) @christianlupus
- l10n: Changed spelling of MIME
  [#988](https://github.com/nextcloud/cookbook/pull/988) @rakekniven
- Move "Categories" caption above list of categories
  [#1000](https://github.com/nextcloud/cookbook/pull/1000) @seyfeb
- Reenable the fixup action after deprecation in central repository
  [#1012](https://github.com/nextcloud/cookbook/pull/1012) @christianlupus
- Trim recipe name to a maximum length to fit in the database
  [#1014](https://github.com/nextcloud/cookbook/pull/1014) @christianlupus
- Correct transifex translations
  [#1024](https://github.com/nextcloud/cookbook/pull/1024) @christianlupus
- Correct singular/plural translations
  [#1026](https://github.com/nextcloud/cookbook/pull/1026) @christianlupus
- Update eslint-plugin-vue
- Fix refresh-icon overlays name of recipe
  [#1033](https://github.com/nextcloud/cookbook/pull/1033) @MarcelRobitaille
- Reenable PR checks from foreign forks
  [#1045](https://github.com/nextcloud/cookbook/pull/1045) @christianlupus
- Prevent access to guzzle client without explicit dependency
  [#1011](https://github.com/nextcloud/cookbook/pull/1011) @christianlupus
- Make PHP code styling more strict
  [#1011](https://github.com/nextcloud/cookbook/pull/1011) @christianlupus
- Adding some strings to transifex
  [#1049](https://github.com/nextcloud/cookbook/pull/1049) @christianlupus
- Removed outdated dependency on v-markdown-editor due to security issues
  [#1050](https://github.com/nextcloud/cookbook/pull/1050) @christianlupus
- Migrated node-sass to dart sass
  [#1051](https://github.com/nextcloud/cookbook/pull/1051) @christianlupus
- Add the url as a parameter to allow for specialized parsers per website in the backend
  [#1060](https://github.com/nextcloud/cookbook/pull/1060) @christianlupus
- Create wrapper in frontend for all API requests
  [#1061](https://github.com/nextcloud/cookbook/pull/1061) @christianlupus

### Removed
- Remove deprecated and no longer functional API routes from app
  [#1065](https://github.com/nextcloud/cookbook/pull/1065) @christianlupus

### Codebase maintenance
- Removed codecov.io upload of intermediate merge commits during pull requests
  [#1028](https://github.com/nextcloud/cookbook/issues/1028)
- Use latest possible NC core for CI tests
- Introduce migration tests
- Enable automatically merging of dependabot PRs
- Add code style checker for package.json
  [#1053](https://github.com/nextcloud/cookbook/pull/1053) @christianlupus
- Remove the amount of data uploaded in CI artifacts
  [#1059](https://github.com/nextcloud/cookbook/pull/1059) @christianlupus
- Outsource of functions from entry files to helper module
  [#1062](https://github.com/nextcloud/cookbook/pull/1062) @christianlupus

### Documentation
- Add documentation on updates of the API endpoints
  [#1001](https://github.com/nextcloud/cookbook/pull/1001) @christianlupus
- Fix API specification in accordance with real implementation
  [#1006](https://github.com/nextcloud/cookbook/pull/1006) @christianlupus

## 0.9.12 - 2022-05-12

### Added
- Add IDE configuration to codebase to prevent small issues
  [#978](https://github.com/nextcloud/cookbook/pull/978) @christianlupus
- Allow client to specify accepted image types
  [#982](https://github.com/nextcloud/cookbook/pull/982) @christianlupus

### Fixed
- Refactor the code for image handling to make it testable
  [#933](https://github.com/nextcloud/cookbook/pull/933) @christianlupus
- Allow merging of PRs from dependabot with only changes to package-lock.json
  [#952](https://github.com/nextcloud/cookbook/pull/952) @christianlupus
- Redirect to login in case of logged out user
  [#956](https://github.com/nextcloud/cookbook/pull/956) @christianlupus
- Correct handling of empty recipe name in the backend
  [#973](https://github.com/nextcloud/cookbook/pull/973) @christianlupus
- Fix problem with git pre-commit hook dropping files unintentionally
  [#974](https://github.com/nextcloud/cookbook/pull/974) @christianlupus
- Removed typo in exception description
  [#965](https://github.com/nextcloud/cookbook/pull/965) @christianlupus
- Mark cookbook app as compatible with NC24
  [#977](https://github.com/nextcloud/cookbook/pull/977) @christianlupus
- Fix bug that prevent generation of thumbnails when no previous thumbnails are present
  [#985](https://github.com/nextcloud/cookbook/pull/985) @christianlupus

### Documentation
- l10n: Corrected some spelling issues
  [#941](https://github.com/nextcloud/cookbook/pull/941) @Valdnet
- Enhanced the user documentation by adding some starter's information
  [#936](https://github.com/nextcloud/cookbook/pull/936) @zorglubu
- Translate user documentation to French
  [#936](https://github.com/nextcloud/cookbook/pull/947) @zorglubu
- Updated French translation
  [#957](https://github.com/nextcloud/cookbook/pull/957) @zorglubu
- Add example to OpenAPI specification
  [#957](https://github.com/nextcloud/cookbook/pull/972) @christianlupus

### Deprecated
- Method RecipeService::parseRecipeHtml()


## 0.9.11 - 2022-03-28

### Fixed
- Reduce complex coupling between event handlers in EditInputGroup.vue
  [#901](https://github.com/nextcloud/cookbook/pull/901) @MarcelRobitaille
- Fix bug in NC Vue config that switches input fields to be not full width on mobile
  [#910](https://github.com/nextcloud/cookbook/pull/910) @MarcelRobitaille
- Enable hot reloading feature of Vue for simpler development
  [#909](https://github.com/nextcloud/cookbook/pull/909) @christianlupus
- Remove some packages from the dependencies to keep the footprint smaller
  [#912](https://github.com/nextcloud/cookbook/pull/912) @christianlupus
- Remove deprecation in preparation for Sass 2.0.0
  [#915](https://github.com/nextcloud/cookbook/pull/915) @MarcelRobitaille
- Fix regression in #900 to allow inserting links to other recipes again
  [#914](https://github.com/nextcloud/cookbook/pull/914) @MarcelRobitaille
- Replace multiple spaces with a single one when pasting
  [#924](https://github.com/nextcloud/cookbook/pull/924) @MarcelRobitaille
- Create abstraction class for access to user configuration
  [#926](https://github.com/nextcloud/cookbook/pull/926) @christianlupus
- Allow unit test to run against webserver with PHP support
  [#927](https://github.com/nextcloud/cookbook/pull/927) @christianlupus
- Enhance the unit test script for more user convinience
  [#931](https://github.com/nextcloud/cookbook/pull/931) @christianlupus

### Documentation
- Introduction about how to start coding
  [#891](https://github.com/nextcloud/cookbook/pull/901) @MarcelRobitaille


## 0.9.10 - 2022-03-04

### Added
- Remove prefix of pasted content for better formatting
  [#887](https://github.com/nextcloud/cookbook/pull/887) @MarcelRobitaille

### Fixed
- Added app info XML back to allow automatic translations
  [#878](https://github.com/nextcloud/cookbook/pull/878) @christianlupus
- Added unit hints in the labels of the timers
  [#879](https://github.com/nextcloud/cookbook/pull/879) @christianlupus
- Allow for multiline text in instructions
  [#880](https://github.com/nextcloud/cookbook/pull/880) @christianlupus
- Usage of caches for NPM speedup
  [#883](https://github.com/nextcloud/cookbook/pull/883) @christianlupus
- Make the controls sticky on top
  [#888](https://github.com/nextcloud/cookbook/pull/888) @MarcelRobitaille
- Cleanup code related to pasting
  [#886](https://github.com/nextcloud/cookbook/pull/886) @MarcelRobitaille
- Make height of control header dependant on server CSS variable
  [#897](https://github.com/nextcloud/cookbook/pull/897) @MarcelRobitaille
- Fix UI glitch when keyword list is empty
  [#892](https://github.com/nextcloud/cookbook/pull/892) @MarcelRobitaille
- Allow switching to new instruction line with Enter key
  [#890](https://github.com/nextcloud/cookbook/pull/890) @MarcelRobitaille
- Prevent inserting newline characters in instructions/ingredients/tools when pressing enter
  [#900](https://github.com/nextcloud/cookbook/pull/900) @MarcelRobitaille

### Documentation
- Added clarification between categories and keywords for users
  [#889](https://github.com/nextcloud/cookbook/pull/889) @MarcelRobitaille


## 0.9.9 - 2022-01-13

### Fixed
- Update NPM plugins to enhance build process
  [#868](https://github.com/nextcloud/cookbook/pull/868) @christianlupus
- Removed missing CSS link in guest template
  [#869](https://github.com/nextcloud/cookbook/pull/869) @christianlupus
- Avoid usage of deprecated JS function
  [#870](https://github.com/nextcloud/cookbook/pull/870) @christianlupus
- Added some translations manually
  (see also [#875](https://github.com/nextcloud/cookbook/issues/875)) @nickvergessen


## 0.9.8 - 2021-12-05

### Fixed
- Update comaptible version to contain v23
  [#864](https://github.com/nextcloud/cookbook/pull/864) @christianlupus


## 0.9.7 - 2021-11-26

### Added
- Add placeholder text to make clear URLs can be used as image source
  [#835](https://github.com/nextcloud/cookbook/pull/835) @seyfeb

### Fixed
- CI build always builds docker images from scratch
  [#823](https://github.com/nextcloud/cookbook/pull/823) @christianlupus
- Fix test script after update in docker-compose
  [#833](https://github.com/nextcloud/cookbook/pull/833) @christianlupus
- Update NPM during automatic building to latest version ([#837](https://github.com/nextcloud/cookbook/issues/837))
  [#839](https://github.com/nextcloud/cookbook/pull/839) @christianlupus
- Downgrade eslint to meet peer dependencies ([#838](https://github.com/nextcloud/cookbook/issues/838))
  [#839](https://github.com/nextcloud/cookbook/pull/839) @christianlupus
- Fix bug in Makefile to simplify development
  [#839](https://github.com/nextcloud/cookbook/pull/839) @christianlupus
- Update eslint and dependencies
  [#848](https://github.com/nextcloud/cookbook/pull/848) @christianlupus
- Update PHP CS-Fixer
  [#849](https://github.com/nextcloud/cookbook/pull/849) @christianlupus
- Update git hooks to not delay commits too much
  [#851](https://github.com/nextcloud/cookbook/pull/851) @christianlupus
- Update git hooks to run all tests even if some fail
  [#856](https://github.com/nextcloud/cookbook/pull/856) @christianlupus
- Make strings recoverable by transifex parser
  [#860](https://github.com/nextcloud/cookbook/pull/860) @christianlupus
- Allow arrays in stored JSON recipe files for the keywords
  [#859](https://github.com/nextcloud/cookbook/pull/859) @christianlupus


## 0.9.6 - 2021-10-18

### Added
- Save button at the bottom of the edit page
  [#818](https://github.com/nextcloud/cookbook/pull/818) @christianlupus

### Fixed
- Usage of PAT for deployment action
  [#815](https://github.com/nextcloud/cookbook/pull/815) @christianlupus
- Correct usage of EXIF data to rotate thumb images accordingly
  [#816](https://github.com/nextcloud/cookbook/pull/816) @christianlupus
- Trim spaces from names of imported recipes
  [#817](https://github.com/nextcloud/cookbook/pull/817) @christianlupus
- Fixed regression in #805
  [#820](https://github.com/nextcloud/cookbook/pull/820) @christianlupus


## 0.9.5 - 2021-10-15

### Fixed
- Fix empty Category
  [#805](https://github.com/nextcloud/cookbook/pull/805) @jotoeri
- Fix CI test scripts
  [#809](https://github.com/nextcloud/cookbook/pull/809) @christianlupus
- Update stylelint-config-prettier
  [#807](https://github.com/nextcloud/cookbook/pull/807) @christianlupus
- Correct unit testing for dependabot and forked branches
  [#811](https://github.com/nextcloud/cookbook/pull/811) @christianlupus
- Updated codecov parser to binary version (fix #810)
  [#813](https://github.com/nextcloud/cookbook/pull/813) @christianlupus
- Allow bot user to push to stable branch
  [#812](https://github.com/nextcloud/cookbook/pull/812) @christianlupus


## 0.9.4 - 2021-09-29

### Fixed
- Failed database caching in case of ill-formatted json file (category/keyword)
  [#797](https://github.com/nextcloud/cookbook/pull/797) @christianlupus
- Added Nook app in README
  [#798](https://github.com/nextcloud/cookbook/pull/798) @christianlupus


## 0.9.3 - 2021-09-26

### Added
- Added unit tests for controllers
  [#790](https://github.com/nextcloud/cookbook/pull/790) @christianlupus
- Added CI test to check for open todo tags in the source code
  [#791](https://github.com/nextcloud/cookbook/pull/791) @christianlupus

### Fixed
- Mark app as compatible with Nextcloud 22
  [#778](https://github.com/nextcloud/cookbook/pull/778) @christianlupus
- Usage of PHAR-based PHPUnit to avoid dependency on nikic/php-parser and dependency conflicts
  [#780](https://github.com/nextcloud/cookbook/pull/780) @christianlupus
- Extracted abstract class for migration testing and added tests code for existing migrations
  [#783](https://github.com/nextcloud/cookbook/pull/783) @christianlupus
- Reactivate step debugging in automated testing
  [#784](https://github.com/nextcloud/cookbook/pull/784) @christianlupus
- Added test result to PR messages
  [#788](https://github.com/nextcloud/cookbook/pull/788) @christianlupus

### Removed
- Removed app info XML file to avoid confusion
  [#778](https://github.com/nextcloud/cookbook/pull/778) @christianlupus


## 0.9.2 - 2021-08-09

### Added
- Added debugging helpers in the CI scripts
  [#774](https://github.com/nextcloud/cookbook/pull/774) @christianlupus

### Fixed
- Fixed changes from #774 and minor extensions
  [#775](https://github.com/nextcloud/cookbook/pull/775) @christianlupus
- Clean tables from old, redundant, and non-unique data to allow migrations (see #762 #763)
  [#776](https://github.com/nextcloud/cookbook/pull/776) @christianlupus


## 0.9.1 - 2021-07-05

### Added
- OpenAPI specification and documentation of the valid API endpoints
  [#757](https://github.com/nextcloud/cookbook/pull/757) @christianlupus

### Fixed
- Correct handling of uploads to codecov
  [#758](https://github.com/nextcloud/cookbook/pull/758) @christianlupus
- Added issue template and documentation regarding website support
  [#759](https://github.com/nextcloud/cookbook/pull/759) @christianlupus
- Avoid sharing of recipes does break the database upgrade process
  [#755](https://github.com/nextcloud/cookbook/pull/755) @christianlupus

### Removed
- Obsolete API routes that are no longer working due to missing files
  [#757](https://github.com/nextcloud/cookbook/pull/757) @christianlupus


## 0.9.0 - 2021-07-01

### Added
- Make recipes searchable through unified search
  [#611](https://github.com/nextcloud/cookbook/pull/611) @PFischbeck
- Enhanced keyword cloud in recipe list with option to hide/show keywords, enlarge area, and ordering alphabetically
  [#678](https://github.com/nextcloud/cookbook/pull/678) @seyfeb
- User documentation
  [#709](https://github.com/nextcloud/cookbook/pull/709) @seyfeb

### Fixed
- Calling reindex
  [#653](https://github.com/nextcloud/cookbook/pull/653) @seyfeb
- Setting nutrition information on recipes with an array assigned for nutrition
  [#653](https://github.com/nextcloud/cookbook/pull/653) @seyfeb
- Fix empty error message upon import
  [#647](https://github.com/nextcloud/cookbook/pull/647) @christianlupus
- Update code styling to match with current version of php-cs-fixer
  [#668](https://github.com/nextcloud/cookbook/pull/668) @christianlupus
- Fix version of `@nextcloud/capabilities` to `1.0.2`
  [#672](https://github.com/nextcloud/cookbook/pull/672) @christianlupus
- Really only show recipe-reference popup on '#'
  [#676](https://github.com/nextcloud/cookbook/pull/676) @seyfeb
- Correct styling of PHP files accoring to php-cs-fixer
  [#692](https://github.com/nextcloud/cookbook/pull/692) @christianlupus
- Removed explicit dependency of @nextcloud/capabilities
  [#693](https://github.com/nextcloud/cookbook/pull/693) @christianlupus
- Add indices to database for all tables
  [#698](https://github.com/nextcloud/cookbook/pull/698) @christianlupus
- Codebase maintenance
  [#699](https://github.com/nextcloud/cookbook/pull/699) @christianlupus
- Enable stalebot
  [#700](https://github.com/nextcloud/cookbook/pull/700) @christianlupus
- Correct error messages when recipe already exists
  [#702](https://github.com/nextcloud/cookbook/pull/702) @christianlupus
- Update webpack version to 5.x
  [#717](https://github.com/nextcloud/cookbook/pull/717) @christianlupus
- Update sass-loader
  [#720](https://github.com/nextcloud/cookbook/pull/720) @christianlupus
- Update compression-webpack-plugin
  [#721](https://github.com/nextcloud/cookbook/pull/721) @christianlupus
- Fix array in recipeYields field according to #722
  [#725](https://github.com/nextcloud/cookbook/pull/725) @christianlupus
- Fix recipe-editor layout as in #729
  [#725](https://github.com/nextcloud/cookbook/pull/732) @seyfeb
- Corrected style of stale bot messages
  [#749](https://github.com/nextcloud/cookbook/pull/749) @christianlupus
- Update the screenshots in the appstore
  [#747](https://github.com/nextcloud/cookbook/pull/747) @mMuck
- Fix visual issues at device width of 1024px #689
  [#751](https://github.com/nextcloud/cookbook/pull/751) @christianlupus
- Removed obsolete dependency on @nextcloud/event-bus
  [#719](https://github.com/nextcloud/cookbook/pull/719) @christianlupus


## 0.8.4 - 2021-03-08

### Added
- Sorting recipes in list by creation and modification date
  [#623](https://github.com/nextcloud/cookbook/pull/623) @seyfeb

### Fixed
- Minor errors in displaying ingredients and instructions
  [#642](https://github.com/nextcloud/cookbook/pull/642) @seyfeb
- Missing translation
  [#644](https://github.com/nextcloud/cookbook/pull/644) @seyfeb
- Recipe-reference popup being shown on the wrong input depending on keyboard layout
  [#648](https://github.com/nextcloud/cookbook/pull/648) @seyfeb

## 0.8.3 - 2021-03-03

### Fixed
- Corrected compatibility list
  [#632](https://github.com/nextcloud/cookbook/pull/632) @christianlupus

## 0.8.2 - 2021-03-03

### Fixed
- Added translation for nutritient-value label placeholder
  [#596](https://github.com/nextcloud/cookbook/pull/596) @seyfeb
- Updated dependency of eslint-config-prettier
  [#603](https://github.com/nextcloud/cookbook/pull/603) @christianlupus
- Enforce basic code styling using prettier in vue files
  [#607](https://github.com/nextcloud/cookbook/pull/607) @christianlupus
- Enforce CSS styling using stylelint
  [#608](https://github.com/nextcloud/cookbook/pull/608) @christianlupus
- More code styling, cleanup & minor bugfixes
  [#615](https://github.com/nextcloud/cookbook/pull/615) @seyfeb
- Avoid daily issues in personal forks due to missing secrets
  [#620](https://github.com/nextcloud/cookbook/pull/620) @christianlupus
- Avoid descending of CS_fixer into non-code folders
  [#621](https://github.com/nextcloud/cookbook/pull/621) @christianlupus
- Fixed compatiblity with Nextcloud 21
  [#605](https://github.com/nextcloud/cookbook/pull/605) @icewind1991

## Deprecated
- Obsolete routes to old user interface, see `appinfo/routes.php`
  [#580](https://github.com/nextcloud/cookbook/pull/580) @christianlupus

## Removed
- Dropped support for NC core version <= 18
  [#630](https://github.com/nextcloud/cookbook/pull/630) @christianlupus

## 0.8.1 - 2021-02-15

### Added
- Code style checker in Vue files
  [#581](https://github.com/nextcloud/cookbook/pull/581) @christianlupus

### Fixed
- Remove look-behind to support Safari users as well
  [#591](https://github.com/nextcloud/cookbook/pull/591) @christianlupus

## 0.8.0 - 2021-02-14

### Added
- Markdown rendering for Description
  [#381](https://github.com/nextcloud/cookbook/pull/381) @thembeat
- Changing category name for all recipes in a category
  [#555](https://github.com/nextcloud/cookbook/pull/555/) @seyfeb
- Functionality to reference other recipes by id in description, tools, ingredients, and instructions
  [#562](https://github.com/nextcloud/cookbook/pull/562/) @seyfeb
- Bundle Analyzer documentation
  [#573](https://github.com/nextcloud/cookbook/pull/573/) @seyfeb
- Added button to allow adding empty ingredient, instruction, and tool entries above existing ones in editor
  [#575](https://github.com/nextcloud/cookbook/pull/575/) @seyfeb

### Changed
- Using computed property in recipe view
  [#522](https://github.com/nextcloud/cookbook/pull/522/) @seyfeb
- Split off list/grid of recipes to separate Vue component
  [#526](https://github.com/nextcloud/cookbook/pull/526/) @seyfeb
- CSS Cleanup, removed central css styling
  [#528](https://github.com/nextcloud/cookbook/pull/528/) @seyfeb
- Timers are hidden when time is zero (prep, cook, total time)
  [#543](https://github.com/nextcloud/cookbook/pull/543/) @seyfeb
- Introduced left navigation pane visibility as Vuex state
  [#544](https://github.com/nextcloud/cookbook/pull/544/) @seyfeb
- Centralized some recipe tasks (create, update, delete)
  [#546](https://github.com/nextcloud/cookbook/pull/546/) @seyfeb
- Added icon for recipes in navigation pane, closes #550
  [#560](https://github.com/nextcloud/cookbook/pull/560/) @seyfeb
- Bumped @nextcloud/vue to 3.5.4
  [#561](https://github.com/nextcloud/cookbook/pull/561/) @seyfeb
- Bump webpack-merge from 4.2.2 to 5.7.3
  [#458](https://github.com/nextcloud/cookbook/pull/458/) @seyfeb
- Bump webpack-cli from 3.3.12 to 4.5.0
  [#565](https://github.com/nextcloud/cookbook/pull/565/)
- Enhanced testing interface
  [#564](https://github.com/nextcloud/cookbook/pull/564) @christianlupus
- Allow guest users to use the cookbook and avoid nextcloud exception handling
  [#506](https://github.com/nextcloud/cookbook/pull/506) @christianlupus

### Fixed
- Added some documentation how to install GH action generated builds
  [#538](https://github.com/nextcloud/cookbook/pull/538) @christianlupus
- Fixed problem where timers are not updated after saving recipe edits
  [#543](https://github.com/nextcloud/cookbook/pull/543/) @seyfeb
- Fixed overlapping misaligned navigation toggles (as in #534)
  [#544](https://github.com/nextcloud/cookbook/pull/544/) @seyfeb
- Refreshing left navigation pane after downloading recipe data, closes #465
  [#547](https://github.com/nextcloud/cookbook/pull/547/) @seyfeb
- Check for existing `@context` setting in json checker
  [#554](https://github.com/nextcloud/cookbook/pull/554) @christianlupus
- Introduced updating recipe directory to Vuex state, fixes #542
  [#546](https://github.com/nextcloud/cookbook/pull/546/) @seyfeb
- Push docker images for different PHP versions
  [#574](https://github.com/nextcloud/cookbook/pull/574) @christianlupus
- Enhanced the CI scripts to be more verbose regarding issues
  [#452](https://github.com/nextcloud/cookbook/pull/452) @christianlupus
- Code cleanup
  [#579](https://github.com/nextcloud/cookbook/pull/579) @christianlupus
- Added label to Dockerfile to be consistent with docker guidelines
  [#582](https://github.com/nextcloud/cookbook/pull/582) @christianlupus
- Corrected jekyll documentation
  [#584](https://github.com/nextcloud/cookbook/pull/584) @christianlupus

### Removed
- Removal of old contoller no longer in use
  [#536](https://github.com/nextcloud/cookbook/pull/536) @christianlupus

## 0.7.10 - 2021-01-16

### Fixed
- Replaced function calls only available in PHP 8 with generic ones
  [#524](https://github.com/nextcloud/cookbook/pull/524) @christianlupus

## 0.7.9 - 2021-01-15

### Changed
- Indentation of ingredients depends on existence of subgroups
  [#512](https://github.com/nextcloud/cookbook/pull/512/) @seyfeb
- Speed up index of recipes by using computed properties
  [#513](https://github.com/nextcloud/cookbook/pull/513) @christianlupus
- Central parsing of parameters for POST/PUT requests to simplify development
  [#518](https://github.com/nextcloud/cookbook/pull/518) @christianlupus
- Removed dependencies on the global jQuery
  [#497](https://github.com/nextcloud/cookbook/pull/497/) @seyfeb

### Fixed
- Fixed keywords of shared recipes counted multiple times, fixes #491
  [#493](https://github.com/nextcloud/cookbook/pull/493/) @seyfeb
- Added basic structure for documentation
  [#499](https://github.com/nextcloud/cookbook/pull/499) @christianlupus
- Make categories load recipes against
  [#500](https://github.com/nextcloud/cookbook/pull/500) @christianlupus
- Handle recipes without category well
  [#501](https://github.com/nextcloud/cookbook/pull/500) @christianlupus
- Allow to save recipes with custom image URLs
  [#505](https://github.com/nextcloud/cookbook/pull/505) @christianlupus
- Allow pasting of instructions without newline again
  [#503](https://github.com/nextcloud/cookbook/pull/503) @christianlupus
- Updated color and bullets in nutrition information, fixes #510
  [#511](https://github.com/nextcloud/cookbook/pull/511/) @seyfeb
- Update README with more clients
  [#457](https://github.com/nextcloud/cookbook/pull/457) @geeseven

## 0.7.8 - 2021-01-08

### Added
- Parse a textual yield field in an imported recipe to a certain degree
  [#327](https://github.com/nextcloud/cookbook/pull/327) @zwoabier
- Search and filter for recipes in the web interface
  [#318](https://github.com/nextcloud/cookbook/pull/318) @sam-19
- CI: Use github actions to check the latest head against unittests
  [#346](https://github.com/nextcloud/cookbook/pull/346) @christianlupus
- CI: Create source code packages for each commit
  [#346](https://github.com/nextcloud/cookbook/pull/346) @christianlupus
- Allow for inconsistent schema: Parse instructions as list of elements
  [#347](https://github.com/nextcloud/cookbook/pull/347) @victorjoos
- Show button to view all recipes without a category
  [#362](https://github.com/nextcloud/cookbook/pull/362/) @seyfeb
- Add a basic changelog to the repository
  [#366](https://github.com/nextcloud/cookbook/pull/366/) @christianlupus
- Enforce update of changelog through CI
  [#366](https://github.com/nextcloud/cookbook/pull/366/) @christianlupus
- Keyword cloud is displayed in recipe
  [#373](https://github.com/nextcloud/cookbook/pull/373/) @seyfeb
- Pasted content with newlines creates new input fields automatically for tools and ingredients in recipe editor
  [#379](https://github.com/nextcloud/cookbook/pull/379/) @seyfeb
- Selectable keywords for filtering in recipe lists
  [#375](https://github.com/nextcloud/cookbook/pull/375/) @seyfeb
- Service to handle schema.org JSON data in strings easier
  [#383](https://github.com/nextcloud/cookbook/pull/383/) @christianlupus
- Unit tests for JSON object service
  [#387](https://github.com/nextcloud/cookbook/pull/387) @TobiasMie
- PHP linter and style checker enabled
  [#390](https://github.com/nextcloud/cookbook/pull/390) @christianlupus
- Automatic deployment of new releases to the nextcloud app store
  [#433](https://github.com/nextcloud/cookbook/pull/433) @christianlupus
- Category and keyword selection from list of existing ones in recipe editor
  [#402](https://github.com/nextcloud/cookbook/pull/402/) @seyfeb
- Allow checking of ingredients in web UI
  [#393](https://github.com/nextcloud/cookbook/pull/393) @christianlupus
- Support for dateCreated and dateModified field of schema.org Recipe
  [#377](https://github.com/nextcloud/cookbook/pull/366/) @seyfeb
- Bundle-Analyzer and Optimization
  [#403](https://github.com/nextcloud/cookbook/pull/403) @thembeat
- Nutrition information display and editing
  [#416](https://github.com/nextcloud/cookbook/pull/416/) @seyfeb
- Asking user for confirmation when leaving recipe-editor form with changes
  [#464](https://github.com/nextcloud/cookbook/pull/464/) @seyfeb
- Exporting the maximal API endpoint version
  [#487](https://github.com/nextcloud/cookbook/pull/487) @christianlupus

### Changed
- Switch of project ownership to nextcloud organization in GitHub
- Change in issue management
- Changes to `.gitignore` file
- Translation issues
- Added available Android apps to README
- Update dev dependencies to recent phpunit to avoid warnings and issues
  [#376](https://github.com/nextcloud/cookbook/pull/376) @christianlupus
- Made the layout more responsive to shift the metadata right of the image in very wide screens
  [#349](https://github.com/nextcloud/cookbook/pull/349/) @christianlupus
- Optimization for SVG to reduce the file size
  [#404](https://github.com/nextcloud/cookbook/pull/404) @thembeat
- Replace Default Recipe-Thumb and Full Image with SVG
  [#418](https://github.com/nextcloud/cookbook/pull/418) @thembeat
- Enhance the CI tests and build valid dist tarballs during the CI runs
  [#435](https://github.com/nextcloud/cookbook/pull/435) @christianlupus
- Images in recipe list are lazily loaded
  [#413](https://github.com/nextcloud/cookbook/pull/413/) @seyfeb
- Improved keyword filtering in recipe lists
  [#408](https://github.com/nextcloud/cookbook/pull/408/) @seyfeb

### Fixed
- Add a min PHP restriction in the metadata
  [#282](https://github.com/nextcloud/cookbook/issues/282) @mrzapp
- Make the codebase consistent with the code standards of the main nextcloud team
  [#295](https://github.com/nextcloud/cookbook/pull/295) @rakekniven
- Improved tooltips of navigation
  [#317](https://github.com/nextcloud/cookbook/pull/317) @sam-19
- Optimize database request for faster access
  [#297](https://github.com/nextcloud/cookbook/pull/297) @christianlupus
- Ignore case during sorting of recipes
  [#333](https://github.com/nextcloud/cookbook/issues/333) @christianlupus
- CI: Repair codecov file paths for correct linkings
  [#348](https://github.com/nextcloud/cookbook/pull/348) @christianlupus
- Make project name compatible with composer 2.0
  [#352](https://github.com/nextcloud/cookbook/pull/352) @christianlupus
- Compress nextcloud logs in case of HTML parsing errors during import
  [#350](https://github.com/nextcloud/cookbook/pull/350) @maxammann
- Make complete sentence in transifex translation from parts
  [#358](https://github.com/nextcloud/cookbook/pull/358) @christianlupus
- Avoid recipe are no longer reachable when user changes locales
  [#371](https://github.com/nextcloud/cookbook/pull/371) @christianlupus
- Hide tooltips in printouts
  [#343](https://github.com/nextcloud/cookbook/pull/343/) @christianlupus
- Creating new recipe not possible due to null reference
  [#378](https://github.com/nextcloud/cookbook/pull/378/) @seyfeb
- Reenabling CI testing with current xdebug 3
  [#417](https://github.com/nextcloud/cookbook/pull/417/) @christianlupus
- Corrected code style in appinfo path
  [#427](https://github.com/nextcloud/cookbook/pull/427) @christianlupus
- Clear filtered keywords when changing the route, fixes #425
  [#426](https://github.com/nextcloud/cookbook/pull/426/) @seyfeb
- Removed typo introduced during refactory cycles
  [#434](https://github.com/nextcloud/cookbook/pull/434) @christianlupus
- Update dependency on code style to version 0.4.x
  [#437](https://github.com/nextcloud/cookbook/pull/437) @christianlupus
- Corrected bugs in CI system
  [#447](https://github.com/nextcloud/cookbook/pull/447) @christianlupus
- Recipe-editing Vue components are not tightly coupled anymore
  [#386](https://github.com/nextcloud/cookbook/pull/386/) @seyfeb
- Fixed trying to remove already removed img DOM nodes in image lazyloading, fixes #462
  [#463](https://github.com/nextcloud/cookbook/pull/463/) @seyfeb
- Fixed cooking time being removed if recipe is saved, fixes #472
  [#473](https://github.com/nextcloud/cookbook/pull/473/) @seyfeb
- Remove keywords from database when a recipe is removed
  [#478](https://github.com/nextcloud/cookbook/pull/478) @christianlupus
- Correct CI to allow creation of releases
  [#482](https://github.com/nextcloud/cookbook/pull/482) @christianlupus
- New version as reported in the API should be saved in the MainController file and thus checked in
  [#488](https://github.com/nextcloud/cookbook/pull/488) @christianlupus

### Removed
- Travis build system
- Support for PHP 7.2
- Removed info button (not) showing the last update time from settings menu, fixes #279
  [#477](https://github.com/nextcloud/cookbook/pull/477/) @seyfeb



## 0.7.7 - 2020-12-10

### Fixed
- Increase version compatibility to nextcloud 20 @mrzapp


## 0.7.6 - 2020-06-27

### Added
- Allow forward slashes in ingredients
  [#272](https://github.com/nextcloud/cookbook/pull/272) @timandrews335

### Fixed
- Swapping ingredients and instructions cause items been deleted
  [#278](https://github.com/nextcloud/cookbook/pull/278) @sam-19
