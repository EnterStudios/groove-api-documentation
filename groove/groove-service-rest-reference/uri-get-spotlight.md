---
title: Discover the Spotlight content API for Groove Music| Groove Services
description:  Get a list of spotlight content in Groove Music catalog with this API
keywords: groove music, groove api, groove new releases, groove spotlight api
author: sakley
ms.assetid: fcee1363-b920-4e8f-a63c-a5ffde7675a8
---

# GET (/1/content/{namespace}/spotlight)
Discover spotlight content for a specified language or culture.

-   [Remarks](#remarks)
-   [Response object](#response-object)
-   [Examples](#examples)

## Remarks
The Spotlight request is composed of mandatory and optional URL parts and query parameters. A request containing all parameters would look like the following string:
```
/1/content/{namespace}/spotlight?language={language}&country={country}

Authorization: Bearer [...]
```

For parameters common to every Groove RESTful API, see [Parameters common to every Groove RESTful API](common-parameters.md). For a table of error codes, see [Error (JSON)](JSON-Error.md). For HTTP status codes, see [Groove RESTful API HTTP Status Codes](http-status-codes.md).

## Response object
[ContentResponse (JSON)](JSON-ContentResponse.md)

## Examples
### Spotlight content
#### Request
```http
GET /1/content/music/spotlight?country=FR&language=FR

Authorization: Bearer [...]
```

#### Response
```json
{
  "Results": {
    "Items": [
      {
        "Type": "Albums",
        "Album": {
          "ReleaseDate": "2014-01-02T00:00:00Z",
          "Duration": "00:55:54",
          "TrackCount": 12,
          "IsExplicit": false,
          "LabelName": "Columbia",
          "Genres": [
            "Rock"
          ],
          "Subgenres": [
            "Indie / Alternative"
          ],
          "AlbumType": "Album",
          "Artists": [
            {
              "Role": "Main",
              "Artist": {
                "Id": "music.0A110000-0200-11DB-89CA-0019B92A3933",
                "Name": "Bruce Springsteen",
                "ImageUrl": "https://musicimage.xboxlive.com/content/music.0A110000-0200-11DB-89CA-0019B92A3933/image?locale=en-US",
                "Link": "https://music.microsoft.com/Artist/0A110000-0200-11DB-89CA-0019B92A3933?partnerID=AwesomePartner",
                "Source": "Catalog"
              }
            }
          ],
          "Id": "music.5FAA1008-0100-11DB-89CA-0019B92A3933",
          "Name": "High Hopes",
          "ImageUrl": "https://musicimage.xboxlive.com/content/music.5FAA1008-0100-11DB-89CA-0019B92A3933/image?locale=en-US",
          "Link": "https://music.microsoft.com/Album/5FAA1008-0100-11DB-89CA-0019B92A3933?partnerID=AwesomePartner",
          "OtherIds": {
            "music.amg": "R  2867329"
          },
          "Source": "Catalog"
        }
      },
      {
        "Type": "Albums",
        "Album": {
          "ReleaseDate": "2013-12-24T00:00:00Z",
          "Duration": "00:43:36",
          "TrackCount": 11,
          "IsExplicit": false,
          "LabelName": "Atlantic Records",
          "Genres": [
            "Rock"
          ],
          "Subgenres": [
            "Indie / Alternative"
          ],
          "AlbumType": "Album",
          "Artists": [
            {
              "Role": "Main",
              "Artist": {
                "Id": "music.847A0000-0200-11DB-89CA-0019B92A3933",
                "Name": "Switchfoot",
                "ImageUrl": "https://musicimage.xboxlive.com/content/music.847A0000-0200-11DB-89CA-0019B92A3933/image?locale=en-US",
                "Link": "https://music.microsoft.com/Artist/847A0000-0200-11DB-89CA-0019B92A3933?partnerID=AwesomePartner",
                "Source": "Catalog"
              }
            }
          ],
          "Id": "music.FD5D0D08-0100-11DB-89CA-0019B92A3933",
          "Name": "Fading West",
          "ImageUrl": "https://musicimage.xboxlive.com/content/music.FD5D0D08-0100-11DB-89CA-0019B92A3933/image?locale=en-US",
          "Link": "https://music.microsoft.com/Album/FD5D0D08-0100-11DB-89CA-0019B92A3933?partnerID=AwesomePartner",
          "OtherIds": {
            "music.amg": "R  2867493"
          },
          "Source": "Catalog"
        }
      },
      {
        "Type": "Albums",
        "Album": {
          "ReleaseDate": "2013-12-19T00:00:00Z",
          "Duration": "00:47:36",
          "TrackCount": 13,
          "IsExplicit": true,
          "LabelName": "Tha Alumni Music Group/88 Classic/RCA Records",
          "Genres": [
            "Hip Hop"
          ],
          "Subgenres": [
            "Contemporary Hip Hop"
          ],
          "AlbumType": "Various Artists Collection",
          "Artists": [
            {
              "Role": "Main",
              "Artist": {
                "Id": "music.F4523800-0200-11DB-89CA-0019B92A3933",
                "Name": "Kid Ink",
                "ImageUrl": "https://musicimage.xboxlive.com/content/music.F4523800-0200-11DB-89CA-0019B92A3933/image?locale=en-US",
                "Link": "https://music.microsoft.com/Artist/F4523800-0200-11DB-89CA-0019B92A3933?partnerID=AwesomePartner",
                "Source": "Catalog"
              }
            }
          ],
          "Id": "music.B9490B08-0100-11DB-89CA-0019B92A3933",
          "Name": "My Own Lane",
          "ImageUrl": "https://musicimage.xboxlive.com/content/music.B9490B08-0100-11DB-89CA-0019B92A3933/image?locale=en-US",
          "Link": "https://music.microsoft.com/Album/B9490B08-0100-11DB-89CA-0019B92A3933?partnerID=AwesomePartner",
          "Source": "Catalog"
        }
      },
      {
        "Type": "Albums",
        "Album": {
          "ReleaseDate": "2014-01-10T00:00:00Z",
          "Duration": "00:03:26",
          "TrackCount": 1,
          "IsExplicit": false,
          "LabelName": "RCA Records Label",
          "Genres": [
            "Pop"
          ],
          "Subgenres": [
            "Contemporary Pop"
          ],
          "AlbumType": "Single",
          "Artists": [
            {
              "Role": "Main",
              "Artist": {
                "Id": "music.8B740000-0200-11DB-89CA-0019B92A3933",
                "Name": "Shakira",
                "ImageUrl": "https://musicimage.xboxlive.com/content/music.8B740000-0200-11DB-89CA-0019B92A3933/image?locale=en-US",
                "Link": "https://music.microsoft.com/Artist/8B740000-0200-11DB-89CA-0019B92A3933?partnerID=AwesomePartner",
                "Source": "Catalog"
              }
            }
          ],
          "Id": "music.93C81508-0100-11DB-89CA-0019B92A3933",
          "Name": "Can't Remember to Forget You",
          "ImageUrl": "https://musicimage.xboxlive.com/content/music.93C81508-0100-11DB-89CA-0019B92A3933/image?locale=en-US",
          "Link": "https://music.microsoft.com/Album/93C81508-0100-11DB-89CA-0019B92A3933?partnerID=AwesomePartner",
          "Source": "Catalog"
        }
      },
      {
        "Type": "Albums",
        "Album": {
          "ReleaseDate": "2013-10-30T00:00:00Z",
          "Duration": "00:33:38",
          "TrackCount": 10,
          "IsExplicit": false,
          "LabelName": "Daptone Records",
          "Genres": [
            "R&B / Soul"
          ],
          "Subgenres": [
            "R&B"
          ],
          "AlbumType": "Album",
          "Artists": [
            {
              "Role": "Main",
              "Artist": {
                "Id": "music.3F060200-0200-11DB-89CA-0019B92A3933",
                "Name": "Sharon Jones & The Dap-Kings",
                "ImageUrl": "https://musicimage.xboxlive.com/content/music.3F060200-0200-11DB-89CA-0019B92A3933/image?locale=en-US",
                "Link": "https://music.microsoft.com/Artist/3F060200-0200-11DB-89CA-0019B92A3933?partnerID=AwesomePartner",
                "Source": "Catalog"
              }
            }
          ],
          "Id": "music.3B8BF507-0100-11DB-89CA-0019B92A3933",
          "Name": "Give the People What They Want",
          "ImageUrl": "https://musicimage.xboxlive.com/content/music.3B8BF507-0100-11DB-89CA-0019B92A3933/image?locale=en-US",
          "Link": "https://music.microsoft.com/Album/3B8BF507-0100-11DB-89CA-0019B92A3933?partnerID=AwesomePartner",
          "OtherIds": {
            "music.amg": "R  2792311"
          },
          "Source": "Catalog"
        }
      },
      {
        "Type": "Albums",
        "Album": {
          "ReleaseDate": "2013-12-05T00:00:00Z",
          "Duration": "01:05:21",
          "TrackCount": 19,
          "IsExplicit": false,
          "LabelName": "Kidz Bop",
          "Genres": [
            "Kids"
          ],
          "Subgenres": [
            "Kids"
          ],
          "AlbumType": "Album",
          "Artists": [
            {
              "Role": "Main",
              "Artist": {
                "Id": "music.2A020100-0200-11DB-89CA-0019B92A3933",
                "Name": "Kidz Bop Kids",
                "ImageUrl": "https://musicimage.xboxlive.com/content/music.2A020100-0200-11DB-89CA-0019B92A3933/image?locale=en-US",
                "Link": "https://music.microsoft.com/Artist/2A020100-0200-11DB-89CA-0019B92A3933?partnerID=AwesomePartner",
                "Source": "Catalog"
              }
            }
          ],
          "Id": "music.BFC80308-0100-11DB-89CA-0019B92A3933",
          "Name": "Kidz Bop 25",
          "ImageUrl": "https://musicimage.xboxlive.com/content/music.BFC80308-0100-11DB-89CA-0019B92A3933/image?locale=en-US",
          "Link": "https://music.microsoft.com/Album/BFC80308-0100-11DB-89CA-0019B92A3933?partnerID=AwesomePartner",
          "Source": "Catalog"
        }
      }
    ]
  }
}
```

### Spotlight for a specific culture
#### Request
```http
GET /1/content/music/spotlight?country=FR&language=FR

Authorization: Bearer [...]
```

#### Response
```json
{
  "Results": {
    "Items": [
      {
        "Type": "Albums",
        "Album": {
          "ReleaseDate": "2014-01-02T00:00:00Z",
          "Duration": "00:55:54",
          "TrackCount": 12,
          "IsExplicit": false,
          "LabelName": "Columbia",
          "Genres": [
            "Alternative"
          ],
          "Subgenres": [
            "Rock Alternatif"
          ],
          "AlbumType": "Album",
          "Artists": [
            {
              "Role": "Main",
              "Artist": {
                "Id": "music.0A110000-0200-11DB-89CA-0019B92A3933",
                "Name": "Bruce Springsteen",
                "ImageUrl": "https://musicimage.xboxlive.com/content/music.0A110000-0200-11DB-89CA-0019B92A3933/image?locale=fr-FR",
                "Link": "https://music.microsoft.com/Artist/0A110000-0200-11DB-89CA-0019B92A3933?partnerID=AwesomePartner",
                "Source": "Catalog"
              }
            }
          ],
          "Id": "music.5FAA1008-0100-11DB-89CA-0019B92A3933",
          "Name": "High Hopes",
          "ImageUrl": "https://musicimage.xboxlive.com/content/music.5FAA1008-0100-11DB-89CA-0019B92A3933/image?locale=fr-FR",
          "Link": "https://music.microsoft.com/Album/5FAA1008-0100-11DB-89CA-0019B92A3933?partnerID=AwesomePartner",
          "OtherIds": {
            "music.amg": "R  2867329"
          },
          "Source": "Catalog"
        }
      },
      {
        "Type": "Albums",
        "Album": {
          "ReleaseDate": "2014-01-02T00:00:00Z",
          "Duration": "00:59:19",
          "TrackCount": 16,
          "IsExplicit": false,
          "LabelName": "Universal Music Division Mercury Records",
          "Genres": [
            "Chanson Française"
          ],
          "Subgenres": [
            "Pop Française"
          ],
          "AlbumType": "Album",
          "Artists": [
            {
              "Role": "Main",
              "Artist": {
                "Id": "music.ABAF5600-0200-11DB-89CA-0019B92A3933",
                "Name": "Yoann Freget",
                "ImageUrl": "https://musicimage.xboxlive.com/content/music.ABAF5600-0200-11DB-89CA-0019B92A3933/image?locale=fr-FR",
                "Link": "https://music.microsoft.com/Artist/ABAF5600-0200-11DB-89CA-0019B92A3933?partnerID=AwesomePartner",
                "Source": "Catalog"
              }
            }
          ],
          "Id": "music.BE021008-0100-11DB-89CA-0019B92A3933",
          "Name": "Quelques Heures Avec Moi",
          "ImageUrl": "https://musicimage.xboxlive.com/content/music.BE021008-0100-11DB-89CA-0019B92A3933/image?locale=fr-FR",
          "Link": "https://music.microsoft.com/Album/BE021008-0100-11DB-89CA-0019B92A3933?partnerID=AwesomePartner",
          "OtherIds": {
            "music.amg": "R  2884867"
          },
          "Source": "Catalog"
        }
      },
      {
        "Type": "Artists",
        "Artist": {
          "Genres": [
            "Alternative"
          ],
          "Subgenres": [
            "Pop Alternative"
          ],
          "Id": "music.CDBE0000-0200-11DB-89CA-0019B92A3933",
          "Name": "Birdy",
          "ImageUrl": "https://musicimage.xboxlive.com/content/music.CDBE0000-0200-11DB-89CA-0019B92A3933/image?locale=fr-FR",
          "Link": "https://music.microsoft.com/Artist/CDBE0000-0200-11DB-89CA-0019B92A3933?partnerID=AwesomePartner",
          "OtherIds": {
            "music.amg": "P  2502969"
          },
          "Source": "Catalog"
        }
      },
      {
        "Type": "Albums",
        "Album": {
          "ReleaseDate": "2013-12-12T00:00:00Z",
          "Duration": "01:10:24",
          "TrackCount": 18,
          "IsExplicit": true,
          "LabelName": "Tha Alumni Music Group/88 Classic/RCA Records",
          "Genres": [
            "Hip Hop / Rap"
          ],
          "Subgenres": [
            "Hip Hop US & Intl."
          ],
          "AlbumType": "Various Artists Collection",
          "Artists": [
            {
              "Role": "Main",
              "Artist": {
                "Id": "music.F4523800-0200-11DB-89CA-0019B92A3933",
                "Name": "Kid Ink",
                "ImageUrl": "https://musicimage.xboxlive.com/content/music.F4523800-0200-11DB-89CA-0019B92A3933/image?locale=fr-FR",
                "Link": "https://music.microsoft.com/Artist/F4523800-0200-11DB-89CA-0019B92A3933?partnerID=AwesomePartner",
                "Source": "Catalog"
              }
            }
          ],
          "Id": "music.DC430808-0100-11DB-89CA-0019B92A3933",
          "Name": "My Own Lane",
          "ImageUrl": "https://musicimage.xboxlive.com/content/music.DC430808-0100-11DB-89CA-0019B92A3933/image?locale=fr-FR",
          "Link": "https://music.microsoft.com/Album/DC430808-0100-11DB-89CA-0019B92A3933?partnerID=AwesomePartner",
          "Source": "Catalog"
        }
      },
      {
        "Type": "Albums",
        "Album": {
          "ReleaseDate": "2013-11-29T00:00:00Z",
          "Duration": "00:40:51",
          "TrackCount": 10,
          "IsExplicit": false,
          "LabelName": "Believe Recordings",
          "Genres": [
            "Alternative"
          ],
          "Subgenres": [
            "Pop Alternative"
          ],
          "AlbumType": "Album",
          "Artists": [
            {
              "Role": "Main",
              "Artist": {
                "Id": "music.18921500-0200-11DB-89CA-0019B92A3933",
                "Name": "James Vincent McMorrow",
                "ImageUrl": "https://musicimage.xboxlive.com/content/music.18921500-0200-11DB-89CA-0019B92A3933/image?locale=fr-FR",
                "Link": "https://music.microsoft.com/Artist/18921500-0200-11DB-89CA-0019B92A3933?partnerID=AwesomePartner",
                "Source": "Catalog"
              }
            }
          ],
          "Id": "music.964A0708-0100-11DB-89CA-0019B92A3933",
          "Name": "Post Tropical",
          "ImageUrl": "https://musicimage.xboxlive.com/content/music.964A0708-0100-11DB-89CA-0019B92A3933/image?locale=fr-FR",
          "Link": "https://music.microsoft.com/Album/964A0708-0100-11DB-89CA-0019B92A3933?partnerID=AwesomePartner",
          "OtherIds": {
            "music.amg": "R  2844041"
          },
          "Source": "Catalog"
        }
      },
      {
        "Type": "Albums",
        "Album": {
          "ReleaseDate": "2013-11-21T00:00:00Z",
          "Duration": "00:03:18",
          "TrackCount": 1,
          "IsExplicit": false,
          "LabelName": "NAIVE",
          "Genres": [
            "R&B / Soul"
          ],
          "Subgenres": [
            "Soul"
          ],
          "AlbumType": "Single",
          "Artists": [
            {
              "Role": "Main",
              "Artist": {
                "Id": "music.F18E0100-0200-11DB-89CA-0019B92A3933",
                "Name": "Anthony Joseph",
                "ImageUrl": "https://musicimage.xboxlive.com/content/music.F18E0100-0200-11DB-89CA-0019B92A3933/image?locale=fr-FR",
                "Link": "https://music.microsoft.com/Artist/F18E0100-0200-11DB-89CA-0019B92A3933?partnerID=AwesomePartner",
                "Source": "Catalog"
              }
            }
          ],
          "Id": "music.9611FE07-0100-11DB-89CA-0019B92A3933",
          "Name": "Tamarind",
          "ImageUrl": "https://musicimage.xboxlive.com/content/music.9611FE07-0100-11DB-89CA-0019B92A3933/image?locale=fr-FR",
          "Link": "https://music.microsoft.com/Album/9611FE07-0100-11DB-89CA-0019B92A3933?partnerID=AwesomePartner",
          "Source": "Catalog"
        }
      }
    ]
  }
}
```

#### Parent
[Groove Service REST Reference](overview.md)
