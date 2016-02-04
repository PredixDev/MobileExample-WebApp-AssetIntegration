# MobileExample-WebApp-AssetIntegration
A sample webapp which displays data from asset service.

## Before You Begin:
It is assumed that you already have running instances of [_Predix Mobile cloud services_](https://www.predix.io/docs#rae4EfJ6) and pushed your [_sync-processor_](https://github.com/PredixDev/MobileExample-Microservice-AssetIntegration) to your CF space (or running on your development system).  

## Configuration

Update `userName` and `assetZoneID` variables in index.html with your _mobile service user_ and _asset service zone id_ resp.

## Installation

Checkout this repository, open the folder in a terminal window, and execute:

```
pm publish
```  
Tip: Checkout _webapp.json_ for app name. And you may need to run `pm publish` based on your _app.json_ configurations.

## Usage
When running on device/simulator it shows three buttons and a text area (in landscape mode atleast).
* [Refresh] - Sends a request to SDK and gets the asset results and updates text area.
* [Watch Changes] - Start watching for changes on asset document and update the text area with new results.
* [PUT] - TODO: Sends changes wrapped in a command document and command-processor will update it in asset service.
