Changelog
=========

---

All notable changes to this project will be documented in this file.<br>
`BFKit Swift` adheres to [Semantic Versioning](http://semver.org/).

---

### 1.x Releases
- `1.6.x` Releases - [1.6.0](#160)
- `1.5.x` Releases - [1.5.0](#150) | [1.5.1](#151)
- `1.4.x` Releases - [1.4.0](#140) | [1.4.1](#141)
- `1.3.x` Releases - [1.3.0](#130) | [1.3.1](#131)
- `1.2.x` Releases - [1.2.0](#120)
- `1.1.x` Releases - [1.1.0](#110)
- `1.0.x` Releases - [1.0.0](#100)

---

## [1.6.0](https://github.com/FabrizioBrancati/BFKit-Swift/releases/tag/v1.6.0) - XX Dec 2015
#### Added
- Added [CONTRIBUTING.md](https://github.com/FabrizioBrancati/BFKit-Swift/blob/master/CONTRIBUTING.md) file
- Added `brightness` directly to UIScreen extension
- Added `randomInt` with range support in NSNumber extension

#### Fixed
- Fixed a bug in `randomColor(_)` that may cause a crash

Thanks to [@Ewg777](https://github.com/Ewg777) for this release



## [1.5.1](https://github.com/FabrizioBrancati/BFKit-Swift/releases/tag/v1.5.1) - 10 Nov 2015
#### Added
- Added more stronger check on BFDataStructures

#### Improved
- Now support Swift 2.1 and Xcode 7.1

#### Fixed
- Fixed a bug in `searchInString(_:charStart:charEnd)` that may cause a crash



## [1.5.0](https://github.com/FabrizioBrancati/BFKit-Swift/releases/tag/v1.5.0) - 5 Nov 2015
#### Added
- Added support for Swift 2.0
- Added `onFirstStartForVersion` and `isFirstStartForVersion` functions and `isFirstStart` and `isFirstStartForCurrentVersion` variables in BFApp class
- Added HEX functions in NSString and String extensions
- Added String functions like URL functions
- Added a `NS` function to String extension that convert it to a NSString
- Added `flipImageHorizontally` & `flipImageVertically` functions in UIImage extension
- Added missing devices

#### Improved
- Now `Array` and `Dictionary` extensions are declared as public
- `indexOfCharacter()` in String extension now doesn't returns `nil` if not found, but `-1`
- Moved `generateUUID()` from UIDevice extension to String and NSString extensions

#### Fixed
- Fixed various bugs



## [1.4.1](https://github.com/FabrizioBrancati/BFKit-Swift/releases/tag/v1.4.1) - 20 Jul 2015
#### Added
- Added support for iPod Touch 6G

#### Fixed
- Fixed a problem with Carthage project



## [1.4.0](https://github.com/FabrizioBrancati/BFKit-Swift/releases/tag/v1.4.0) - 13 Jul 2015
#### Added
- Added `APP_DELEGATE` global variable
- Added UINavigationBar extension
- Added UIToolbar & UIBarButtonItem extensions
- Added BFDataStructures class with primitive data structures
- Added new substring, indexOf and subscript functions in String extension
- Added `fallbackTitle` parameter in `showTouchIDAuthenticationWithReason` function in BFTouchID class
- Added touch on screen with `BFShowTouchOnScreen()` and `BFHideTouchOnScreen()` functions

#### Improved
- Removed UIScreen functions from UIDevice extension and created UIScreen extension
- Changed `SCREEN_WIDTH` & `SCREEN_HEIGHT` variables and fixed [#2](https://github.com/FabrizioBrancati/BFKit-Swift/issues/2) (Thanks to [jiongge](https://github.com/jiongge))

#### Fixed
- Fixed `iOSVersion` function in UIDevice extension



## [1.3.1](https://github.com/FabrizioBrancati/BFKit-Swift/releases/tag/v1.3.1) - 9 Jul 2915
#### Added
- Added `onFirstStart` and `onFirstStartForCurrentVersion` in BFApp class
- Added `stringByReplacingWithRegex:withString:` in NSString and String extensions

#### Improved
- BFLog now prints: `timestamp filename:line function message`
- NSDate extension now has `nanosecond` and use `autoupdatingCurrentCalendar`
- Bug fix in DEMO App



## [1.3.0](https://github.com/FabrizioBrancati/BFKit-Swift/releases/tag/v1.3.0) - 7 Jul 2015
#### Added
- Added a DEMO App
- Added `init(imageAsTemplate:, tintColor:)` to create UIImageView with a template image
- Added a new init function in UIColor extension to create UIColor with an HEX in Int
- Added function `dictionaryToJSON` and deprecated the old one in NSDictionary extension
- Added `moveObjectFromIndex` function in NSMutableArray extension

#### Improved
- NSThread extension is now public and can perform selectors in background
- `BFLocalizedString` now doesn't require `comment` parameter
- Changed `BFLogString` and `BFDetailedLogString` from functions to variables
- `showTouchIDAuthenticationWithReason` in BFTouchID class now returns `result` in closure
- In some UIKit extension the delegate (or data source) can now be `nil`
- `searchCharStart` functions in NSString extension now requires a NSString for start and end
- Changed how to check if is an email in NSString and String extensions
- `colorForColorString` has been moved from UIImage to UIColor extension
- Renamed `image` variable to `screenshot` in `takeScreenshotWithDelay` function in UIWindow extension
- Marked some function as obsoleted

#### Fixed
- Fixed a bug with `iOSVersion` function in UIDevice extension
- Fixed a bug with all the CIFilter in UIImage extension
- Fixed a bug in `deleteFile` function in NSFileManager extension
- Fixed a bug in `safeSetObject` function in NSMutableDictionary extension



## [1.2.0](https://github.com/FabrizioBrancati/BFKit-Swift/releases/tag/v1.2.0) - 5 Jul 2015
#### Added
- Added comments to all classes and extensions
- Added the documentation with [CocoaDocs](http://cocoadocs.org/docsets/BFKit-Swift/)

#### Improved
- Declared public `colorForColorString` in UIColor extension
- Declared as deprecated some functions in favor of default values



## [1.1.0](https://github.com/FabrizioBrancati/BFKit-Swift/releases/tag/v1.1.0) - 2 Jul 2015
#### Added
- Added Carthage support
- Added all IDs in BFSystemSound class
- Added all font family names and font names in UIFont extension

#### Improved
- Now you can use word like `red`, `blue` or any predefined color in UIColor class to create dummy images with `UIColor(dummyImageWithSizeAndColor:)`
- Changed `loadArrayToPath` to `loadArrayFromPath` and now return `AnyObject?`
- Removed `cpuUsage` function in NSProcessInfo extension
- Reverted to old `BFLog` function in BFLog class

#### Fixed
- Fixed `dictionaryToJson:` in Dictionary extension



## [1.0.0](https://github.com/FabrizioBrancati/BFKit-Swift/releases/tag/v1.0.0) 30 Jun 2015
- Initial release
