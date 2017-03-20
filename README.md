# MMM-NASA

A MagicMirror module to display the Earth as it rotates.

## What you see and how you see it.
NASA's EPIC camera, aboard NOAA's DSCOVR satellite. NASA's Earth Polychromatic Imaging Camera (EPIC) instrument provides daily, full disc imagery of the Earth and captures unique perspectives of certain astronomical events such as lunar transits using a 2048x2048 pixel CCD (Charge Coupled Device) detector coupled to a 30-cm aperture Cassegrain telescope.



## Dependencies

* An installation of [MagicMirror<sup>2</sup>](https://github.com/MichMich/MagicMirror)
* npm
* [request](https://www.npmjs.com/package/request)


## Info

* No API key is necessary but these limits apply.
* 30 requests per IP address per hour
* 50 requests per IP address per day.

## Installation

* Clone this repo into `~/MagicMirror/modules` directory.
* `cd MMM-NASA`
* `npm install` in ~/MagicMirror/modules/MMM-NASA directory.

## Add to Config.js

    ```
    {
        module: "MMM-NASA",
        position: "top_center",
        config: {
            header: "",
            MaxWidth: "50%",
            MaxHeight: "50%",
            ...
        }
    },
    ```

## Config Options

| **Option** | **Default** | **Description** |
| --- | --- | --- |
| `updateInterval` | `10 * 360000` (1 hour) | How often should the data be fetched in ms. |
| `animationSpeed` | `1000` | The speed at which the module loads in ms. |
| `initialLoadDelay` | `2500` | Module load delay in ms |
| `retryDelay` | `2500` |Delay to retry fetching data. |
| `useHeader` | true |Set this to bool value true or false. Must be set to true if you use header |
| `header` | `""` | Add header between the `""` if desired. |
| `MaxWidth` | `""`|  Choose width of image between the `""` (Ex: `200px` or '12%'). |
| `MaxHeight` | `""` | Choose height of image between the `""` (Ex: `200px` or '12%').. |

