# Swift Checkout V2 Automation

## Getting Started
- ### Installing Dependencies

To run this automation you need to install some dependencies and module as system requirements.


| Name | Download Link |
| ------ | ------ |
| Python                    | [Download](https://www.python.org/downloads/)             |
| VSCode IDE (`Optional`)   | [Download](https://code.visualstudio.com/download)        |
| Git                       | [Download](https://git-scm.com/downloads)                 |
|Google Chrome              | [Download](https://www.google.com/chrome/)                |
|Chrome Driver              | [Download](https://chromedriver.chromium.org/downloads)   |

> Note :  Please download `Chrome Driver` as same as your Google Chrome Version. You can check more guide for installing `Chrome Driver` through this [Link](https://chromedriver.chromium.org/downloads)

- ### Installing Module (`Python Required!`)
> Note :  To install this module you have to run this command via `Command Line Aplication` on your Sistem Operation
- `Windows`   : Command Prompt OR Windows Power Shell
- `Mac`       : Terminal Command
- `Linux`     : Command Line

##### List Modules

- Robot Framework
```sh
pip install robotframework
```

- Selenium Library for Robot framework
```sh
pip install robotframework-seleniumlibrary
```

- Faker Library for Robot Framework
```sh
pip install robotframework-faker
```

## Clone Project
> Note :  To clone this repository you have to run this command via `Command Line Aplication` and `Git` has been installed on your Sistem Operation. You can clone this project on your own folder or partition.
- Clone Swift Checkout V2 Automation
```sh
git clone https://github.com/icube-mage/swift-checkout-v2-automation.git
git checkout develop
```

## Running Project
> Note : You can only running this project via `Command Line Application`.
- Running all test
```sh
robot test
```

- Running specific test
```sh
robot test/[Name Files]
```
> Note : `Name Files` means file name inside `test` folder, example : `01_ecp_shopping_cart.robot`

- Running specific tags
```sh
robot -i [Tag Name] test
```
> Note : `Tag Name` means all test case that have specific tag from all of test case, example : if you want to run only `checkout` case, you can just type command `robot -i checkout test`. This command include `ecp` and `dashboard` tag, you can find more when you read the files one by one.

## Project Structure
- ### Overview
![N|Solid](https://raw.githubusercontent.com/yudha1121/Readme/main/SS%20Documentation/all.png)
- Swift Checkout V2 Automation is created with Three main folders which name is `base`,`pages`,`resources`, and `test`. 

![N|Solid](https://raw.githubusercontent.com/yudha1121/Readme/main/SS%20Documentation/base.png)
- Folder `base` and `pages` is contain **Keyword** which is use for **Test Case**. 

![N|Solid](https://raw.githubusercontent.com/yudha1121/Readme/main/SS%20Documentation/data.png)
- Folder `resources`is contain **Variable** which is use for **Test Case** and **Form Operation**.

![N|Solid](https://raw.githubusercontent.com/yudha1121/Readme/main/SS%20Documentation/test.png)
- Folder `test` is contain **Test Case** which is use for testing the behavior of web application.

## Log & Report
![N|Solid](https://raw.githubusercontent.com/yudha1121/Readme/main/SS%20Documentation/reports.png) <br>
After running test, you can see the result through `Log.html` AND `Report.html` files, you can find both of files inside `Project Folder` where you clone it.

#### Test Result
![N|Solid](https://raw.githubusercontent.com/yudha1121/Readme/main/SS%20Documentation/pass.png)<br>
 - **PASS** : All test that get **PASS** result means the test that have been run is expected output
 

![N|Solid](https://raw.githubusercontent.com/yudha1121/Readme/main/SS%20Documentation/fail.png)
 - **FAILED** : All test that get **FAILED** result means the test that have been run is unexpected output

#### Tips
![N|Solid](https://raw.githubusercontent.com/yudha1121/Readme/main/SS%20Documentation/tips.png)
> Note : You can find `FAILED` part from the result through screenshot from the `Log.html` files.
