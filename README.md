# Turbolinks iOS Template

## Quick Setup
* Check out this project
* Run `pod install` in your terminal
* Open `SmigglesIOS.xcworkspace` (not `SmigglesIOS.xcodeproj`)
* Profit

## Installation
Install Turbolinks manually by building Turbolinks.framework and linking it to your project.

**Installing with CocoaPods**
Add the following to your `Podfile`:
```
use_frameworks!
pod 'Turbolinks', :git => 'https://github.com/turbolinks/turbolinks-ios.git'
```
Then run `pod install` in your terminal.

# ROR Setup/Tips
You will need to make the following changes to your ROR app to work with Turbolinks iOS in a usable manor.
* Implement `TurbolinksNativeMessageHandler` JS
* All forms MUST be submitted `remote: true`
* Handle redirection from JS with `Turbolinks.visit("<%= j your_path %>");`
* Do not use modals (especially CSS only modals), use individual pages.
