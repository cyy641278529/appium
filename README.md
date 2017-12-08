# Appium samples

Simulate touch input by appium

## Install

```bash
npm install appium
brew install carthage
```
## Download appium-xcuitest-driver

https://github.com/facebook/WebDriverAgent

## Configure WDA

```bash
  cd /Users/yourname/WebDriverAgent
  mkdir -p Resources/WebDriverAgent.bundle
  sh ./Scripts/bootstrap.sh
```

open  `WebDriverAgent.xcodeproj`
     WebDriverAgentLib->Build Setting->Runpath Search Paths->Add variable：

     `$(SRCROOT)/../Carthage/Build/iOS`
     `$(PROJECT)/Carthage/Build/iOS`

then WebDriverAgentLib->Build Setting->Build Active Architecture Only->No
 build and test
 Product -> Destination -> iphone6（choice simulator）
Scheme  -> WebDriverAgentRunner:  Product -> Scheme ->WebDriverAgentRunner
 Product -> Test
