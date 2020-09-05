# <img src="https://github.com/woeplanet-data/woeplanet-data/raw/master/assets/woe.png" width="32" height="32">&nbsp;woeplanet-data

> "Everything is related to everything else, but near things are more related than distant things.”
>
> &mdash;<cite>[Tobler’s First Law of Geography](https://www.geolounge.com/toblers-first-law-geography/)</cite>

## The Short Version

WoePlanet is WhereOnEarth (AKA WOE) (AKA Geoplanet) data, based on Yahoo's GeoPlanet Data download, with some, but not all, of the original hierarchy linkages reinstated, with some, but not all, centroid and polygon coordinates added in from other data sources and formatted as GeoJSON, one file per WOEID and organised by Geoplanet place type.

Per-country and per-placetype repositories exist as part of the GitHub [`woeplanet`](https://github.com/woeplanet-data) organisation, with the following naming convention ...

```
woeplanet-[placetype]-[iso 3166-2 code]
```

So data for placetype `8` (state) for the United Kingdom would live in the following repo ...

```
woeplanet-state-gb
```

In some cases, even with splitting repos by placetype and country, the repo is getting close to GitHub's theoretical maximum repo size. In this case the data is further sub-partitioned, based on the first character of the place's name, so data for placetype `11` (zip) for the United Kingdom starting with `A` lives in the following repo ...

```
woeplanet-zip-gb-a
```

## Who's On First?

Any similarity between Woeplanet and [Who's On First](https://www.whosonfirst.org/) is entirely coincidental. Inspiration for Who's On First came from Geoplanet, Yahoo's (now defunct) global gazetter and inspiration for Woeplanet came from Who's On First, especially on repository naming conventions and GeoJSON properties.

# The Long(er) Version

_Forking GeoPlanet one place at a time ..._

This is an active but still experimental project to create a community driven project to maintain, update and make public in a usable form the Creative Commons licensed GeoPlanet data set.

Right at the very start was a set of closely coupled software and data called GeoPlanet, developed by UK based GDC (Graphical Data Capture). The heart of GeoPlanet was a hierarchically linked set of geographic place definitions, so for any place you could determine all the language and colloquial name variants, the parent(s), the children and adjacent or neighbouring places. Each entry in GeoPlanet was assigned a unique 32-bit identifier, known as a _Whereonearth ID_, or _WOEID_. GDC was subsequently acquired by Whereonearth in 1998 with the software component rebranded as InternetLocality and the data retaining the GeoPlanet name.

In 2005, Whereonearth was itself acquired by Yahoo!, initially to form part of the internal search marketing program, internally named as Panama. Four years later, as part of the Yahoo! Developer Network, a set of APIs based on InternetLocality were publicly released as GeoPlanet and Placemaker. To avoid confusion over the use of the GeoPlanet name, the data set was internally rebranded as WhereHaüs (pun fully intentional) and GeoPlanet was used solely to refer to the API. Coincident to this, a version of the data set was released publicly under a CC-BY license as GeoPlanet Data.

GeoPlanet Data contained some of the hierarchical richness of the internal data, including parent and adjacent relationships, but omitted child, sibling, "belongsto" and ancestor relationships. All geospatial data, such as centroids, polygons and bounding boxes were also removed due to licensing restrictions from third party, proprietary data sources.

The GeoPlanet Data set continued to be maintained and updated until June 2012 when Yahoo! removed access to the downloads with a message saying _We are currently making the data non-downloadable while we determine a better way to surface the data as a part of the service_. This remained until mid 2015 when Yahoo! announced that the YDN GeoPlanet and Placemaker APIs would be shutting down, although equivalent functionality would be available via the YQL API and the BOSS Geo APIs. The GeoPlanet API finally shut down late in 2016 and YQL was shutdown in early 2019. The BOSS Geo APIs are currently still available behind the BOSS paywall.

The publicly released GeoPlanet Data dumps remain available via the [Internet Archive](https://archive.org/search.php?query=subject%3A%22geoplanet%22) and several projects were released to make use of the data, such as [GPLplanet](https://github.com/twbell/GPLplanet) by ex-Yahoo! Geo Director or Product Tyler Bell and [woedb](https://web.archive.org/web/20180308192417/http://woe.spum.org/) by ex-Flickr Lead Engineer Aaron Straup Cope, who went on to be one of the founding team members behind Who's on First. woedb went offline in 2018 and that was the genesis of WoePlanet.

# See also ...

* [woedb](https://www.aaronland.info/weblog/2010/04/05/milkshake/#woedb)
* [twbell/GPLplanet](https://github.com/twbell/GPLplanet)
