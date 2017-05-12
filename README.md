# Swift Library for EmojiOne


[![CocoaPods](https://img.shields.io/cocoapods/v/EmojiOne.svg)](http://cocoadocs.org/docsets/EmojiOne)  [![Platform](https://img.shields.io/cocoapods/p/EmojiOne.svg)](http://cocoadocs.org/docsets/EmojiOne)  ![Swift](https://img.shields.io/badge/%20in-swift%203.0-orange.svg)

[![Travis](https://img.shields.io/travis/ranesr/EmojiOne.svg)](https://travis-ci.org/ranesr/EmojiOne/)


Please &#9733; this library.

This EmojiOne library helps you use icons from [EmojiOne](https://emojione.com).

EmojiOne library currently supports `UIImageView` and `UILabel`.


## Requirements

- iOS 8.0+
- Xcode 8


## Installation


### Cocoapods

[CocoaPods](http://cocoapods.org) is a dependency manager for Cocoa projects.

Make sure you have the latest version of CocoaPods by running:

```bash
$ gem install cocoapods
# (or if the above fails)
$ sudo gem install cocoapods
```

Update your local specs repo by running:

```bash
$ pod repo update
```

Add the following lines to your `Podfile`:

```ruby
target 'YourAwesomeProject' do
    use_frameworks!
    pod 'EmojiOne'
end
```

Then run the following command

```bash
$ pod install
```

You can start using the library by importing it wherever you want

```swift
import EmojiOne
```


### Swift Package Manager

You can use [The Swift Package Manager](https://swift.org/package-manager) to install `EmojiOne` by adding the proper description to your `Package.swift` file:

```swift
import PackageDescription

let package = Package(
    name: "YourAwesomeProject",
    targets: [],
    dependencies: [
        .Package(url: "https://github.com/ranesr/EmojiOne", majorVersion: 1)
    ]
)
```

Note that the [Swift Package Manager](https://swift.org/package-manager) is still in early design and development, for more information checkout its [GitHub Page](https://github.com/apple/swift-package-manager)


### Manually

Copy the file from `Sources` folder.

[Link to file](https://github.com/ranesr/EmojiOne/tree/master/Sources).


## Usage


### UIImageView

```Swift

// Setting emoji to image view
imageView.setEmoji(.speechLeft)
imageView.setEmoji(.womanRowingBoat)

```

### UILabel

```Swift

// Setting emoji to label
label.setEmoji("PREFIX TEXT ", .manFarmerTone4, " POSTFIX TEXT")
label.setEmoji("", .flashlight, " POSTFIX TEXT")
label.setEmoji("PREFIX TEXT ", .cruiseShip, "")

```

## Author

Saurabh Rane

- [Email](mailto:saurabhrrane@gmail.com)
- [LinkedIn](https://linkedin.com/in/ranesaurabh)

## Licence

EmojiOne is available under the MIT License. See the `LICENSE` file for more info.
