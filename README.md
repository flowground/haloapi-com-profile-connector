# ![LOGO](logo.png) Profile **flow**ground Connector

## Description

A generated **flow**ground connector for the Profile API (version 1.0).

Generated from: https://api.apis.guru/v2/specs/haloapi.com/profile/1.0/swagger.json<br/>
Generated at: 2019-05-07T17:42:14+03:00

## API Description

API that provides Profile information about Players.

## Authorization

Supported authorization schemes:
- API Key- API Key
## Actions

### Halo 5 - Player Appearance

> <p>This Endpoint retrieves appearance information for a player.</p><br/>
> <p>If the player is a member of a Company, the Company's ID and Name will be provided. Additional Company information is available via the Stats API.</p><br/>
> <br /><br/>
> <h4>Changelog</h4><br/>
> <div class="panel-body"><br/>
>     <p><strong>July 14, 2017:</strong></p><br/>
>     <ul><br/>
>         <li>Added Endpoint.</li><br/>
>     </ul><br/>
> </div>

#### Input Parameters
* `player` - _required_ - The Player's Gamertag

### Halo 5 - Player Emblem Image

> <p>This Endpoint returns an HTTP Redirect (302 Found) response to the caller with the URL of an image of the Player's Emblem. The initial request to this API that returns the HTTP Redirect is throttled and requires a Subscription Key. However, the image itself (at hostname "image.halocdn.com") is not throttled and does not require a Subscription Key. Note that if the Player later changes their Emblem, the image itself is not refreshed and will need to be refreshed via a new request to this API.</p><br/>
> <br /><br/>
> <h4>Changelog</h4><br/>
> <div class="panel-body"><br/>
>     <p><strong>July 14, 2017:</strong></p><br/>
>     <ul><br/>
>         <li>Renamed Endpoint from "Halo 5 - Emblem Image" to "Halo 5 - Player Emblem Image".</li><br/>
>     </ul><br/>
>     <p><strong>February 21, 2017:</strong></p><br/>
>     <ul><br/>
>         <li>Renamed Endpoint from "Emblem Image" to "Halo 5 - Emblem Image".</li><br/>
>         <li>Removed "{title}" Request Parameter.</li><br/>
>     </ul><br/>
> </div>

#### Input Parameters
* `player` - _required_ - The Player's Gamertag.
* `size` - _optional_ - An optional size (specified in pixels) of the image requested. When specified, this value must be one of the following values: 95, 128, 190, 256, 512. If a value is specified that is not in this list, the API returns HTTP 400 ("Bad Request"). If the size is empty or missing, the API will use 256.

### Halo 5 - Player Spartan Image

> <p>This Endpoint returns an HTTP Redirect (302 Found) response to the caller with the URL of an image of the Player's Spartan's appearance. The initial request to this API that returns the HTTP Redirect is throttled and requires a Subscription Key. However, the image itself (at hostname "image.halocdn.com") is not throttled and does not require a Subscription Key. Note that if the Player later changes their Spartan's appearance, the image itself is not refreshed and will need to be refreshed via a new request to this API.</p><br/>
> <br /><br/>
> <h4>Changelog</h4><br/>
> <div class="panel-body"><br/>
>     <p><strong>July 14, 2017:</strong></p><br/>
>     <ul><br/>
>         <li>Renamed Endpoint from "Halo 5 - Spartan Image" to "Halo 5 - Player Spartan Image".</li><br/>
>     </ul><br/>
>     <p><strong>February 21, 2017:</strong></p><br/>
>     <ul><br/>
>         <li>Renamed Endpoint from "Spartan Image" to "Halo 5 - Spartan Image".</li><br/>
>         <li>Removed "{title}" Request Parameter.</li><br/>
>     </ul><br/>
> </div>

#### Input Parameters
* `player` - _required_ - The Player's Gamertag.
* `size` - _optional_ - An optional size (specified in pixels) of the image requested. When specified, this value must be one of the following values: 95, 128, 190, 256, 512. If a value is specified that is not in this list, the API returns HTTP 400 ("Bad Request"). If the size is empty or missing, the API will use 256.
* `crop` - _optional_ - An optional crop that will be used to determine what portion of the Spartan is returned in the image. The value must be either "full" or "portrait". If no value is specified "full" is used. If an unsupported value is provided, the API returns HTTP 400 ("Bad Request").

## License

**flow**ground :- Telekom iPaaS / haloapi-com-profile-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
