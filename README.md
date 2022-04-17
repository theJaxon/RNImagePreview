# RNImagePreview
Using a simple cocoapod for image previews in React Native

### react-native upgrade to 0.29.0

### Details
* See [here](https://medium.com/infinite-red/beginner-s-guide-to-using-cocoapods-with-react-native-46cb4d372995#.1qx1m22bh) for full blog post
* See [here](https://medium.com/infinite-red) for all publications from Infinite Red 

## Getting started

_(These instructions assume that you already have ReactNative and CocoaPods set up on your machine)_

1. Read the blog post linked above
2. Clone the repo to your computer
3. `cd` into the `RNImagePreview` directory and run `npm install`
5. `cd` into the `ios` directory and run `pod install`
6. Open the `RNImagePreview.xcworkspace` file (or if you have the awesome [`open_pod_bay`](https://github.com/leshill/open_pod_bay) gem installed you can just type `pod open`)
7. Press `CMD`+`R` or click the run button in XCode to build and run the project


---

### Azure DevOps Pipelines
#### azure-pipelines.yml
- Executes the instructions specified in Getting Started Section 
- Adds Rugby for Cocoapods Caching
- Caches rugby, Pods and node dependencies

#### [azure-parallel.yml](https://cloudaffaire.com/how-to-create-and-execute-azure-pipelines-using-rest-api/)
- Runs 2 Pipelines in Parallel Via [API](https://docs.microsoft.com/en-us/rest/api/azure/devops/pipelines/runs/run-pipeline?view=azure-devops-rest-6.0)

### References
- [How to create and execute Azure Pipelines using REST API?](https://cloudaffaire.com/how-to-create-and-execute-azure-pipelines-using-rest-api/)
- [Cache CocoaPods for faster rebuild and indexing Xcode project](https://github.com/swiftyfinch/Rugby)