# Patkai
Interface and GeoJSON data for historical and modern-day villages in the Patkai range. This project has two purposes:

1. To provide an accurate historical record of village locations and migrations of the Tangsa, Nocte, Ollo and related groups through and from the Patkai mountains.
2. To better contextualise linguistic change that has happened in the region over the past centuries.

The former is being done through a combination of digitisation of old survey maps of the region and conversations with those who've made the migrations or recall stories from their elders. Through this, the latter will be beneficial in providing a clearer indication of when and where language contact has occurred between groups. Members of the communities are also able to get in touch digitally over Facebook or on-side messaging to offer corrections and suggestions.

As part of this endeavour, we're also continuing to make improvements on the OpenStreetMap data for the area, especially in terms of waterways and mountain names which may assist in locating historical sites.

## Historical sources

British Survey maps:
* 83M, ~1923, Japanese reprint
* 83M/SE, published 1927 under E.A. Tandy
* 83M/SE, 1927, Japanese reprint
* 83N/NE, published 1934 under H.J. Couchman
* 83N/NW, ~1930, Japanese reprint
* 83N/SE, published 1930 under R.H. Thomas
* 92A/3, 1926, Japanese reprint
* 92B/NW, published 1923 under C.H.D. Ryder
* 92B/SW, ~1923, Japanese reprint

US Army Corps of Engineers maps:
* NG46-4 Dibrugarh, 1957
* NG46-4 Dibrugarh, 1967
* NG46-8 Sibsagar, 1957
* NG46-8 Sibsagar, 1967
* NG47-1 Putao, 1957
* NG47-1 Putao, 1967

Additional sources of information acquired through personal communications, 2015-present

## Example documents
The following are examples of a MongoDB document for a single village. The first is for a village which appears on a number of maps, with additional data confirmed by someone from the region.

```javascript
{
    _id: ObjectId("58918113ebcacc3e0c0041b1"),
    confirmed: true,
    coord: [
        27.101463,
        95.9314155
    ],
    display: {
        color: "rgba(0,0,0,0.4)"
    },
    properties: {
        group: "Mueshaung",
        label: "Ghaqsawz Kanx"
    },
    sources: [
        {
            date: 1927,
            group: "",
            label: "Hasingkān",
            source: "83M/SE",
            sourcename: "Tandy"
        },
        {
            date: 1957,
            group: "",
            label: "Hasingkān",
            source: "NG46-4"
        },
        {
            date: 1967,
            group: "",
            label: "Hasingkān",
            source: "NG46-4"
        }
    ]
}
```

Some villages were both founded and abandoned in between the periods during which surveys were made. Otherws have life spans which can be approximated, or founding dates that are clearly known. For such locations, lifespan dates are also given:

```javascript
    life: {
        start: 1960,
        stop: 1985
    },
```

## Sample screenshot
![](http://phonemica.net/github/patkai.jpg)
