# Patkai
Interface and GeoJSON data for historical and modern-day villages in the Patkai range. This project has two purposes:

1. To provide an accurate historical record of village locations and migrations of the Tangsa, Nocte, Ollo and related groups through and from the Patkai mountains.
2. To better contextualise linguistic change that has happened in the region over the past centuries.

The former is being done through a combination of digitisation of old survey maps of the region and conversations with those who've made the migrations or recall stories from their elders. Through this, the latter will be beneficial in providing a clearer indication of when and where language contact has occurred between groups. Members of the communities are also able to get in touch digitally over Facebook or on-side messaging to offer corrections and suggestions.

As part of this endeavour, we're also continuing to make improvements on the OpenStreetMap data for the area, especially in terms of waterways and mountain names which may assist in locating historical sites.

## Example document
The following is an example of a MongoDB document for a single village.

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

## Sample screenshot
![](http://phonemica.net/github/patkai.jpg)
