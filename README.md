# StreamKit

The StreamKit project is intended to showcase [DonorDrive API](https://github.com/DonorDrive/PublicAPI) best practices in a collection of utilities designed to help charity stream fundraising campaigns. The StreamKit leverages [Vue](https://vuejs.org/), [Axios](https://github.com/axios/axios), [Moment.js](https://momentjs.com), [Numeral.js](numeraljs.com), [Animate.css](https://animate.style/) and [Bootstrap](https://getbootstrap.com).

## Getting Started

To download the StreamKit, you'll want to hit the green Code button on the screen and click 'Download Zip'. Unzip the folder to your desired location.

Navigate to the folder and locate config.js, once found, right click on this file and hit "Open with", you'll want to open it with Notepad.

Once notepad is open with the file, locate resourceID and enter in your participant ID here. Make sure to save and you'll be all set to use these tools.

## `config.js`

`config.js` serves as a single reference point to inform StreamKit widgets where to look for information, as well as their look and feel. The 3 properties that must be set are:

- `api` - the url of the DonorDrive API you wish to poll
- `resource` - the resource (events, participants, teams)
- `resourceID` - the ID of the specific resource to poll

## `donation-ticker`

`donation-ticker` takes advantage of the `etag` returned from an initial call to a resource before making a subsequent call to retrieve new/recent donations.

## `streaming-alerts`

`streaming-alerts` offers a quick shout-out to donors, giving the opportunity for more central placement within a stream.

## `streaming-thermometer`

`streaming-thermometer` is a persistent element that tracks fundraising progress against your goal in DonorDrive. Donation alerts are enabled by default, but may be disabled if this is used in conjunction with `streaming-alerts` (set `streamingThermometer.showDonations` to `false`).
