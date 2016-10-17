# MobileExample-WebApp-AssetIntegration
A sample web app that displays data from asset service.

## Before You Begin:
It is assumed that you have running instances of [_Predix Mobile service_](https://www.predix.io/docs#rae4EfJ6) and [_Predix Asset service_](https://www.predix.io/docs/#aRPNr2R9), and you have installed the Predix Mobile pm command line tool.  
It is also assumed that you have pushed your [_sync-processor_](https://github.com/PredixDev/MobileExample-Microservice-AssetIntegration) to your CF space (or have it running on your development system). 

To get started, follow this documentation:
* [Get Started with the Mobile Service and Mobile SDK] (https://www.predix.io/docs#rae4EfJ6) 
* [Running the Predix Mobile Sample App] (https://www.predix.io/docs#EGUzWwcC)
* [Creating a Mobile Hello World Web App] (https://www.predix.io/docs#DrBWuHkl) 


## Configuration

Update `userName` and `assetZoneID` variables in `index.html` with your _mobile service user_ and _asset service zone id_ respectively.

## Installation

Checkout this repository, open the folder in a terminal window, and execute:

```
pm publish
```  
Tip: Checkout `webapp.json` for the app name. And, you might need to run `pm publish` based on your `app.json` configuration.

## Usage
When running on a device/simulator, the app shows two buttons and a text area (when in landscape mode).
* [Refresh] - Sends a request to SDK and gets the asset results and updates text area.
* [Watch Changes] - Start watching for changes on asset document and update the text area with new results.

