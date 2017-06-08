# <img src="assets/woe.png" width="64" height="64" alt="woeplanet">&nbsp;woeplanet-data

> "Everything is related to everything else, but near things are more related than distant things.”
>
> &mdash;<cite>[Tobler’s First Law of Geography](https://www.geolounge.com/toblers-first-law-geography/)</cite>

## The Short Version

`woeplanet` is WhereOnEarth (AKA WOE) (AKA GeoPlanet) data, based on Yahoo's now defunct GeoPlanet Data download, with the original hierarchy linkages reinstated and formatted as GeoJSON, one file per WOEID and organised by GeoPlanet place type.

## Show Me The Data

GitHub has this to say about [repository sizes](https://help.github.com/articles/what-is-my-disk-quota/) ...

> We recommend repositories be kept under 1GB each. This limit is easy to stay within if large files are kept out of the repository. If your repository exceeds 1GB, you might receive a polite email from GitHub Support requesting that you reduce the size of the repository to bring it back down.

As the total size (at the time of writing) of the `woeplanet` data is > XXX GB, the data is split into repos by place type, or, when even that makes the repo too big, by place type and ISO 3166-1 alpha 2 country code.

This means there's quite a few repos. ~750 at the current count.

_Sorry_.

* woeplanet-airport
* woeplanet-colloquial
* woeplanet-continent
* woeplanet-country
* woeplanet-county
* woeplanet-drainage
* woeplanet-estate
* woeplanet-historical-county
* woeplanet-historical-state
* woeplanet-historical-town
* woeplanet-island
* woeplanet-land-feature-[iso-country-code]
* woeplanet-local-admin
* woeplanet-local-admin-[iso-country-code]
* woeplanet-misc
* woeplanet-ocean
* woeplanet-poi-[iso-country-code]
* woeplanet-sea
* woeplanet-sports-team
* woeplanet-state
* woeplanet-suburb
* woeplanet-suburb-[iso-country-code]
* woeplanet-supername
* woeplanet-timezone
* woeplanet-town-[iso-country-code]
* woeplanet-unknown
* woeplanet-zip-[iso-country-code]
* woeplanet-zone
