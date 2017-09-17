# Font Awesome in Swift
Font Awesome is a Free Icon Package which gives you variety of Icons. Whether you're in Android, iOS or Web, it supports all of them.

### Features
* Single Source File
* No Need to refers the Icons unicode. It'll give you the *suggestion*
* Customize icon's color and size
* Import *ttf* file and You're done.

### Steps
1. Import font-awesome *fontawesome.ttf* file in your project and mention it in your Project's Info.plist file.
2. Font Awesome Icons are implicitly are the characters so, every Icon are UILable type.
3. In Our case, You need to assign UILabel as SwiftFontAwesome type in your File Inspector.

  ```swift
    @IBOutlet weak var myLabel: SwiftFontAwesome!
  ```

  And, there you call icon(type: withSize:) method

  ```swift

  //Set Icon
  myLabel.icon(type: .ambulance, withSize: .tripleExtraLarge)

  ```

  Here, *type:* is the name of Icon which belong to type *FontAwesomeIcon* enum.
  And, withSize: decides the size of icon.

  ##### Icons Sizes,
  * customSize (Default is 10)
  * extraSmall (12)
  * small (14)
  * medium (16)
  * large (18)
  * extraLarge (20)
  * doubelExtraLarge (24)
  * tripleExtraLarge (32)

4. With Color Customization,

  ```swift

    myLabel.icon(type: .sortAmountAsc, withSize: .large, withColor: .green, shadowColor: .blue)

  ```

### Feature Request or Bugs
Please post any bugs to the issue tracker found on the project's GitHub page.
