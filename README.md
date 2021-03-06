[![Maintainability](https://api.codeclimate.com/v1/badges/b81f96d501e3f41bf2cc/maintainability)](https://codeclimate.com/github/milespratt/bingmaps-react/maintainability) <a href="https://codeclimate.com/github/milespratt/bingmaps-react/test_coverage"><img src="https://api.codeclimate.com/v1/badges/b81f96d501e3f41bf2cc/test_coverage" /></a> [![Build Status](https://travis-ci.com/milespratt/bingmaps-react.svg?branch=master)](https://travis-ci.com/milespratt/bingmaps-react)

<img align="right" width="100" height="100" src="https://github.com/milespratt/bingmaps-react/blob/master/src/assets/logo.png?raw=true">

# Bing Maps - React

An easy to use Bing Maps component for React apps. View the [demo](https://bingmaps-react.netlify.com).

<!-- <p align="center"> -->
  <img align="center" width="500" height="500" src="https://github.com/milespratt/bingmaps-react/blob/master/src/assets/screenshot.png?raw=true">
<!-- </p> -->

## Prerequisites

You must have a Bing Maps API key to take full advantage of this component. You can obtain an API key from the [Bing Maps Dev Center](https://www.bingmapsportal.com).

## Installation

`npm install bingmaps-react`

## Usage

Import the BingMapsReact component.

```javascript
import BingMapsReact from "bingmaps-react";
```

Render the component, passing in your bing maps API key

```javascript
<BingMapsReact credentials="YOUR BING MAPS API KEY" />
```

Example:

```javascript
import React from "react";
import BingMapsReact from "bingmaps-react";

function MyReactApp() {
  return (
    <div>
      <BingMapsReact credentials="YOUR BING MAPS API KEY" />
    </div>
  );
}
```

## Available Props

#### Component Specific

| Prop      | Type   | Default     |
| --------- | ------ | ----------- |
| className | string | bing\_\_map |
| id        | string | bing_map_0  |

#### Bing Maps Specific

Each of these props control one of the Bing Maps Map Options. See the [MapOptions Object documentation](https://docs.microsoft.com/en-us/bingmaps/v8-web-control/map-control-api/mapoptions-object) for more information about each option.

| Prop                            | Type    | Default   |
| ------------------------------- | ------- | --------- |
| credentials                     | string  | undefined |
| customMapStyle                  | string  | undefined |
| disableBirdseye                 | boolean | false     |
| disableMapTypeSelectorMouseOver | boolean | false     |
| disableStreetside               | boolean | false     |
| disableStreetsideAutoCoverage   | boolean | false     |
| enableClickableLogo             | boolean | true      |
| navigationBarMode               | string  | default   |
| showDashboard                   | boolean | true      |
| showMapTypeSelector             | boolean | true      |
| showScalebar                    | boolean | true      |
| showTermsLink                   | boolean | true      |
