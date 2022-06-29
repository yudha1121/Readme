# Swift Automation
#
## Getting Started
- ### Installing Dependencies

To run this automation you need to install some dependencies and module as system requirements.


| Name | Download Link |
| ------ | ------ |
| Python                    | [Download](https://www.python.org/downloads/)             |
| VSCode IDE (`Optional`)   | [Download](https://code.visualstudio.com/download)        |
| Git                       | [Download](https://git-scm.com/downloads)                 |
| Google Chrome             | [Download](https://www.google.com/chrome/)                |
| Chrome Driver             | [Download](https://chromedriver.chromium.org/downloads)   |

> Note :  Please download `Chrome Driver` as same as your Google Chrome Version. You can check more guide for installing `Chrome Driver` through this [Link](https://github.com/icube-mage/swift-checkout-v2-automation/blob/538dc5f0037961c9ec420359db0ce259d74369d7/ChromDriver.md)

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

## Clone Project
> Note :  To clone this repository you have to run this command via `Command Line Aplication` and `Git` has been installed on your Sistem Operation. You can clone this project on your own folder or partition.
- Clone Swift Automation
```sh
git clone https://github.com/icube-mage/swift-automation-test.git
git checkout develop
```

## Running Project

- `Running all test`

> SH File :
```sh
Open : `auto.sh` inside project folder.
```

`OR`

> Command Line :
```sh
robot robot
```

- `Running daily test`
> Note : Daily test is useful for send daily report and usually this test is general condition of customer behavior

> SH File :
```sh
Open : `daily.sh` inside project folder.
```

`OR`

> Command Line :
```sh
robot -i daily robot
```

- `Running specific tags`
```sh
robot -i [Tag Name] robot
```
![N|Solid](https://github.com/yudha1121/Readme/blob/main/SS%20Documentation/tag.png)
> Note : `Tag Name` means all test case that have specific tag from all of test case, example : if you want to run only `checkout` case, you can just type command `robot -i checkout robot`. There is more tag like `daily` tag that can be useful to run specific test, you can find more when you read the files inside `robot` folder one by one.

- `Running specific test file`
```sh
robot robot/[Name Files]
```
> Note : `Name Files` means file name inside `robot` folder, example : `01Register.robot`


## Project Structure
- ### Overview
![N|Solid](https://raw.githubusercontent.com/yudha1121/Readme/main/SS%20QA%20Swift/all.png)
- Swift Automation is created with Two main folders which name is `resource`, and `robot`.

![N|Solid](https://raw.githubusercontent.com/yudha1121/Readme/main/SS%20QA%20Swift/resources.png)
- Folder `resource` is contain **Keyword, Locator, String, and Variable (TestData)** which is use for **Test Case**. 

![N|Solid](https://raw.githubusercontent.com/yudha1121/Readme/main/SS%20QA%20Swift/robot.png)
- Folder `robot` is contain **Test Case** which is use for testing the behavior of web application.

## Log & Report
![N|Solid](https://raw.githubusercontent.com/yudha1121/Readme/main/SS%20QA%20Swift/result-sh.png)<br>
After running test especially using `SH files` like `daily.sh` OR `auto.sh`, you can see the result through `Log.html` AND `Report.html` inside `result` folder, you can find it inside specific `time` folder when you run the test. Example : `22Jun2022-145111`

![N|Solid](https://raw.githubusercontent.com/yudha1121/Readme/main/SS%20QA%20Swift/result-reg.png)<br>
After running test throught `Command Line`, you can see the result through `Log.html` AND `Report.html` files, you can find both of files inside `Project Folder` where you clone it.

## Test Result
![N|Solid](https://raw.githubusercontent.com/yudha1121/Readme/main/SS%20QA%20Swift/pass.png)<br>
 - **PASS** : All test that get **PASS** result means the test that have been run is expected output
 

![N|Solid](https://raw.githubusercontent.com/yudha1121/Readme/main/SS%20QA%20Swift/fail.png)
 - **FAILED** : All test that get **FAILED** result means the test that have been run is unexpected output

#### Tips
![N|Solid](https://raw.githubusercontent.com/yudha1121/Readme/main/SS%20QA%20Swift/tips.png)
> Note : You can find `FAILED` part from the result through screenshot from the `Log.html` files.
