
# AndroidAppLockscreen
An easily implementable, clean, minimal Lockscreen module for Android Apps. Design inspired by Diary ( https://play.google.com/store/apps/details?id=com.pixelcrater.Diaro )

# Screenshots

Image1                     |  Image2
:-------------------------:|:-------------------------:
![screenshot_1532237234](https://user-images.githubusercontent.com/6418354/43042536-7e991234-8da2-11e8-8d17-f15c963a6ad2.png)  | ![screenshot_1532237239](https://user-images.githubusercontent.com/6418354/43042543-a5326274-8da2-11e8-8a96-31e84eef0c98.png)

[![](https://badgen.net/github/release/p32929/AndroidAppLockscreen)]() [![](https://badgen.net/github/release/p32929/AndroidAppLockscreen/stable)]() [![](https://badgen.net/github/tag/p32929/AndroidAppLockscreen)]() [![](https://badgen.net/github/watchers/p32929/AndroidAppLockscreen)]() [![](https://badgen.net/github/checks/p32929/AndroidAppLockscreen)]() [![](https://badgen.net/github/status/p32929/AndroidAppLockscreen)]() [![](https://badgen.net/github/stars/p32929/AndroidAppLockscreen)]() [![](https://badgen.net/github/forks/p32929/AndroidAppLockscreen)]() [![](https://badgen.net/github/issues/p32929/AndroidAppLockscreen)]() [![](https://badgen.net/github/open-issues/p32929/AndroidAppLockscreen)]() [![](https://badgen.net/github/closed-issues/p32929/AndroidAppLockscreen)]() [![](https://badgen.net/github/label-issues/p32929/AndroidAppLockscreen/help-wanted/open)]() [![](https://badgen.net/github/prs/p32929/AndroidAppLockscreen)]() [![](https://badgen.net/github/open-prs/p32929/AndroidAppLockscreen)]() [![](https://badgen.net/github/closed-prs/p32929/AndroidAppLockscreen)]() [![](https://badgen.net/github/merged-prs/p32929/AndroidAppLockscreen)]() [![](https://badgen.net/github/commits/p32929/AndroidAppLockscreen)]() [![](https://badgen.net/github/last-commit/p32929/AndroidAppLockscreen)]() [![](https://badgen.net/github/branches/p32929/AndroidAppLockscreen)]() [![](https://badgen.net/github/releases/p32929/AndroidAppLockscreen)]() [![](https://badgen.net/github/tags/p32929/AndroidAppLockscreen)]() [![](https://badgen.net/github/license/p32929/AndroidAppLockscreen)]() [![](https://badgen.net/github/contributors/p32929/AndroidAppLockscreen)]() [![](https://badgen.net/github/dependents-pkg/p32929/AndroidAppLockscreen)]() 

## Share
Sharing with your friends is just one click away from here

[![facebook](https://image.flaticon.com/icons/png/32/124/124010.png)](https://www.facebook.com/sharer/sharer.php?u=https://github.com/p32929/AndroidAppLockscreen)
[![twitter](https://image.flaticon.com/icons/png/32/124/124021.png)](https://twitter.com/intent/tweet?source=https://github.com/p32929/AndroidAppLockscreen)
[![tumblr](https://image.flaticon.com/icons/png/32/124/124012.png)](https://www.tumblr.com/share?v=3&u=https://github.com/p32929/AndroidAppLockscreen)
[![pocket](https://image.flaticon.com/icons/png/32/732/732238.png)](https://getpocket.com/save?url=https://github.com/p32929/AndroidAppLockscreen)
[![pinterest](https://image.flaticon.com/icons/png/32/124/124039.png)](https://pinterest.com/pin/create/button/?url=https://github.com/p32929/AndroidAppLockscreen)
[![reddit](https://image.flaticon.com/icons/png/32/2111/2111589.png)](https://www.reddit.com/submit?url=https://github.com/p32929/AndroidAppLockscreen)
[![linkedin](https://image.flaticon.com/icons/png/32/1409/1409945.png)](https://www.linkedin.com/shareArticle?mini=true&url=https://github.com/p32929/AndroidAppLockscreen)
[![whatsapp](https://image.flaticon.com/icons/png/32/733/733585.png)](https://api.whatsapp.com/send?text=https://github.com/p32929/AndroidAppLockscreen)

## Support
If you like my works and want to support me/my works, feel free to support or donate. My payment details can be found here: https://p32929.github.io/SendMoney2Me/

## Installation
Add it in your root build.gradle at the end of repositories:

```
allprojects {
  repositories {
    maven { url 'https://jitpack.io' }
  }
}
```

Add the dependency

```
dependencies {
    implementation 'com.github.p32929:AndroidAppLockscreen:1.2'
}
```

## Usage
Steps to follow:
* Extend all ``Activities`` by ``LockscreenHandler``
* Add ```EasyLock.checkPassword(this);``` in your ```MainActivity```'s ```onCreate``` method (or whichever activity starts at first)

After that you can:
* Set password
* Set background color
* Check password
* Change password
* Disable password

## Example:
Step 1: * Extend all ``Activities`` by ``LockscreenHandler`` like this:

```
public class MainActivity extends LockscreenHandler {
   // ............................................
}
```

Step 2: Add ```EasyLock.checkPassword(this);``` in your ```MainActivity```'s ```onCreate``` method (or whichever activity starts at first) like this:

```
@Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);

        EasyLock.checkPassword(this);
}
```

## Set, Check, Change, Disable Password:
* To set a password, call ```EasyLock.setPassword();```
* To set background color, call ```EasyLock.setBackgroundColor();```
* To check password, call ```EasyLock.checkPassword();```
* To change password, call ```EasyLock.changePassword();```
* To disable password, call ```EasyLock.disablePassword();```
* To see if clicked on Forgot password call ```EasyLock.forgotPassword()``` with a ```new View.OnClickListener()```

Check out the app in the repository for more info :)
Enjoy...

```
MIT License

Copyright (c) 2018 Fayaz Bin Salam

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```
