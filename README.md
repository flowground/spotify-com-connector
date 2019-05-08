# ![LOGO](logo.png) Spotify **flow**ground Connector

## Description

A generated **flow**ground connector for the Spotify API (version v1).

Generated from: https://api.apis.guru/v2/specs/spotify.com/v1/swagger.json<br/>
Generated at: 2019-05-07T17:44:10+03:00

## API Description



## Authorization

Supported authorization schemes:
- OAuth2
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### [Get Several Albums](https://developer.spotify.com/web-api/get-several-albums/)

#### Input Parameters
* `ids` - _required_ - A comma-separated list of IDs
* `market` - _optional_ - The market (an ISO 3166-1 alpha-2 country code)

### [Get an Album](https://developer.spotify.com/web-api/get-album/)

#### Input Parameters
* `id` - _required_ - The Spotify ID for the album
* `market` - _optional_ - The market (an ISO 3166-1 alpha-2 country code)

### [Get an Album's Tracks](https://developer.spotify.com/web-api/get-albums-tracks/)

#### Input Parameters
* `id` - _required_ - The Spotify ID for the album
* `limit` - _optional_ - The maximum number of items to return
* `offset` - _optional_ - The index of the first item to return
* `market` - _optional_ - The market (an ISO 3166-1 alpha-2 country code)

### [Get Several Artists](https://developer.spotify.com/web-api/get-several-artists/)

#### Input Parameters
* `ids` - _required_ - A comma-separated list of IDs

### [Get an Artist](https://developer.spotify.com/web-api/get-artist/)

#### Input Parameters
* `id` - _required_ - The Spotify ID for the artist

### [Get an Artist's Albums](https://developer.spotify.com/web-api/get-artists-albums/)

#### Input Parameters
* `id` - _required_ - The Spotify ID for the artist
* `limit` - _optional_ - The maximum number of items to return
* `offset` - _optional_ - The index of the first item to return
* `album_type` - _optional_ - Filter by album types
* `market` - _optional_ - The market (an ISO 3166-1 alpha-2 country code)

### [Get an Artist's Related Artists](https://developer.spotify.com/web-api/get-related-artists/)

#### Input Parameters
* `id` - _required_ - The Spotify ID for the artist

### [Get an Artist's Top Tracks](https://developer.spotify.com/web-api/get-artists-top-tracks/)

#### Input Parameters
* `id` - _required_ - The Spotify ID for the artist
* `country` - _required_ - The country (an ISO 3166-1 alpha-2 country code)

### [Get a List of Browse Categories](https://developer.spotify.com/web-api/get-list-categories/)

#### Input Parameters
* `limit` - _optional_ - The maximum number of items to return
* `offset` - _optional_ - The index of the first item to return
* `country` - _optional_ - The country (an ISO 3166-1 alpha-2 country code)
* `locale` - _optional_ - The desired language, consisting of an ISO 639 language code and an ISO 3166-1 alpha-2 country code, joined by an underscore. For example: es_MX, meaning "Spanish (Mexico)".

* `Accept` - _optional_ - It is used to set specified media type.

### [Get a Single Browse Category](https://developer.spotify.com/web-api/get-category/)

#### Input Parameters
* `category_id` - _required_ - The Spotify ID of the category you wish to fetch.
* `country` - _optional_ - The country (an ISO 3166-1 alpha-2 country code)
* `locale` - _optional_ - The desired language, consisting of an ISO 639 language code and an ISO 3166-1 alpha-2 country code, joined by an underscore. For example: es_MX, meaning "Spanish (Mexico)".

* `Accept` - _optional_ - It is used to set specified media type.

### [Get a Category's playlists](https://developer.spotify.com/web-api/get-categorys-playlists/)

#### Input Parameters
* `category_id` - _required_ - The Spotify ID of the category you wish to fetch.
* `limit` - _optional_ - The maximum number of items to return
* `offset` - _optional_ - The index of the first item to return
* `country` - _optional_ - The country (an ISO 3166-1 alpha-2 country code)
* `Accept` - _optional_ - It is used to set specified media type.

### [Get a List of Featured Playlists](https://developer.spotify.com/web-api/get-list-featured-playlists/)

#### Input Parameters
* `limit` - _optional_ - The maximum number of items to return
* `offset` - _optional_ - The index of the first item to return
* `country` - _optional_ - The country (an ISO 3166-1 alpha-2 country code)
* `locale` - _optional_ - The desired language, consisting of an ISO 639 language code and an ISO 3166-1 alpha-2 country code, joined by an underscore. For example: es_MX, meaning "Spanish (Mexico)".

* `timestamp` - _optional_ - A timestamp in ISO 8601 format (yyyy-MM-dd'T'HH:mm:ss) with the user's local time to get results tailored to a specific date and time in the day. If not provided, it defaults to the current UTC time. Example: "2014-10-23T09:00:00" for a user whose local time is 9AM.

* `Accept` - _optional_ - It is used to set specified media type.

### [Get a List of New Releases](https://developer.spotify.com/web-api/get-list-new-releases/)

#### Input Parameters
* `limit` - _optional_ - The maximum number of items to return
* `offset` - _optional_ - The index of the first item to return
* `country` - _optional_ - The country (an ISO 3166-1 alpha-2 country code)
* `Accept` - _optional_ - It is used to set specified media type.

### [Get Current User's Profile](https://developer.spotify.com/web-api/get-current-users-profile/)

### [Unfollow Artists or Users](https://developer.spotify.com/web-api/unfollow-artists-users/)

#### Input Parameters
* `type` - _required_ - The type to unfollow.
    Possible values: artist, user.
* `ids` - _required_ - A comma-separated list of the artists or users ids

### [Get User's Followed Artists](https://developer.spotify.com/web-api/get-followed-artists/)

#### Input Parameters
* `type` - _required_ - The ID type, currently only artist is supported.
    Possible values: artist.
* `limit` - _optional_ - The maximum number of items to return
* `after` - _optional_ - The last artist ID retrieved from the previous request.

### [Follow Artists or Users](https://developer.spotify.com/web-api/follow-artists-users/)

#### Input Parameters
* `type` - _required_ - The type to follow.
    Possible values: artist, user.
* `ids` - _required_ - A comma-separated list of the artists or users ids

### [Check if Current User Follows Artists or Users](https://developer.spotify.com/web-api/check-current-user-follows/)

#### Input Parameters
* `type` - _required_ - The type to follow.
    Possible values: artist, user.
* `ids` - _required_ - A comma-separated string of the artists or users ids.

### [Remove Tracks for Current User](https://developer.spotify.com/web-api/remove-tracks-user/)

#### Input Parameters
* `ids` - _required_ - A comma-separated list of IDs
* `Accept` - _optional_ - It is used to set specified media type.

### [Get Current User's Saved Tracks](https://developer.spotify.com/web-api/get-users-saved-tracks/)

#### Input Parameters
* `limit` - _optional_ - The maximum number of items to return
* `offset` - _optional_ - The index of the first item to return
* `market` - _optional_ - The market (an ISO 3166-1 alpha-2 country code)
* `Accept` - _optional_ - It is used to set specified media type.

### [Save Tracks for Current User](https://developer.spotify.com/web-api/save-tracks-user/)

#### Input Parameters
* `ids` - _required_ - A comma-separated list of IDs
* `Accept` - _optional_ - It is used to set specified media type.

### [Check Current User's Saved Tracks](https://developer.spotify.com/web-api/check-users-saved-tracks/)

#### Input Parameters
* `ids` - _required_ - A comma-separated list of IDs

### [Search for an Item](https://developer.spotify.com/web-api/search-item/)

#### Input Parameters
* `limit` - _optional_ - The maximum number of items to return
* `offset` - _optional_ - The index of the first item to return
* `q` - _required_ - The search query's keywords (and optional field filters). The search is not case-sensitive: 'roadhouse' will match 'Roadhouse', 'roadHouse', etc. Keywords will be matched in any order unless surrounded by quotes, thus q=roadhouse&20blues will match both 'Blues Roadhouse' and 'Roadhouse of the Blues'. Quotation marks can be used to limit the match to a phrase: q=roadhouse&20blues will match 'My Roadhouse Blues' but not 'Roadhouse of the Blues'. By default, results are returned when a match is found in any field of the target object type. Searches can be made more specific by specifying an album, artist or track field filter. For example q=album:gold%20artist:abba&type=album will search for albums with the text 'gold' in the album name and the text 'abba' in an artist name. Other possible field filters, depending on object types being searched, include year, genre, upc, and isrc. For example, q=damian%20genre:reggae-pop&type=artist. The asterisk (*) character can, with some limitations, be used as a wildcard (maximum: 2 per query). It will match a variable number of non-white-space characters. It cannot be used in a quoted phrase, in a field filter, or as the first character of the keyword string. Searching for playlists will return results matching the playlist's name and/or description.
* `type` - _required_ - A comma-separated list of item types to search across. Search results will include hits from all the specified item types; for example q=name:abacab&type=album,track will return both albums and tracks with "abacab" in their name.
* `market` - _optional_ - The market (an ISO 3166-1 alpha-2 country code).  If given, only items with content playable in that market will be returned.

### [Get Several Tracks](https://developer.spotify.com/web-api/get-several-tracks/)

#### Input Parameters
* `ids` - _required_ - A comma-separated list of IDs
* `market` - _optional_ - The market (an ISO 3166-1 alpha-2 country code)

### [Get a Track](https://developer.spotify.com/web-api/get-track/)

#### Input Parameters
* `id` - _required_
* `market` - _optional_ - The market (an ISO 3166-1 alpha-2 country code)

### [Get a User's Profile](https://developer.spotify.com/web-api/get-users-profile/)

#### Input Parameters
* `user_id` - _required_ - The user's Spotify user ID.

### [Get a List of a User's Playlists](https://developer.spotify.com/web-api/get-list-users-playlists/)

#### Input Parameters
* `user_id` - _required_ - The user's Spotify user ID.
* `limit` - _optional_ - The maximum number of items to return
* `offset` - _optional_ - The index of the first item to return
* `Accept` - _optional_ - It is used to set specified media type.

### [Create a Playlist](https://developer.spotify.com/web-api/create-playlist/)

#### Input Parameters
* `user_id` - _required_ - The user's Spotify user ID.
* `Accept` - _optional_ - It is used to set specified media type.

### [Get a Playlist](https://developer.spotify.com/web-api/get-playlist/)

#### Input Parameters
* `user_id` - _required_ - The user's Spotify user ID.
* `playlist_id` - _required_ - The Spotify playlist ID.
* `fields` - _optional_ - A comma-separated list of fields to filter query
* `market` - _optional_ - The market (an ISO 3166-1 alpha-2 country code)
* `Accept` - _optional_ - It is used to set specified media type.

### [Change a Playlist's Details](https://developer.spotify.com/web-api/change-playlist-details/)

#### Input Parameters
* `user_id` - _required_ - The user's Spotify user ID.
* `playlist_id` - _required_ - The Spotify playlist ID.
* `Accept` - _optional_ - It is used to set specified media type.

### [Unfollow a Playlist](https://developer.spotify.com/web-api/unfollow-playlist/)

#### Input Parameters
* `user_id` - _required_ - The user's Spotify user ID.
* `playlist_id` - _required_ - The Spotify playlist ID.

### [Follow a Playlist](https://developer.spotify.com/web-api/follow-playlist/)

#### Input Parameters
* `user_id` - _required_ - The user's Spotify user ID.
* `playlist_id` - _required_ - The Spotify playlist ID.

### [Check if Users Follow a Playlist](https://developer.spotify.com/web-api/check-user-following-playlist/)

#### Input Parameters
* `user_id` - _required_ - The user's Spotify user ID.
* `playlist_id` - _required_ - The Spotify playlist ID.
* `ids` - _required_ - A comma-separated list of users ids

### [Remove Tracks from a Playlist](https://developer.spotify.com/web-api/remove-tracks-playlist/)

#### Input Parameters
* `user_id` - _required_ - The user's Spotify user ID.
* `playlist_id` - _required_ - The Spotify playlist ID.
* `Accept` - _optional_ - It is used to set specified media type.

### [Get a Playlist's Tracks](https://developer.spotify.com/web-api/get-playlists-tracks/)

#### Input Parameters
* `user_id` - _required_ - The user's Spotify user ID.
* `playlist_id` - _required_ - The Spotify playlist ID.
* `limit` - _optional_ - The maximum number of items to return
* `offset` - _optional_ - The index of the first item to return
* `fields` - _optional_ - A comma-separated list of fields to filter query
* `market` - _optional_ - The market (an ISO 3166-1 alpha-2 country code)
* `Accept` - _optional_ - It is used to set specified media type.

### [Add Tracks to a Playlist](https://developer.spotify.com/web-api/add-tracks-to-playlist/)

#### Input Parameters
* `user_id` - _required_ - The user's Spotify user ID.
* `playlist_id` - _required_ - The Spotify playlist ID.
* `position` - _optional_ - The position to insert the tracks, a zero-based index
* `uris` - _required_ - A comma-separated list of Spotify track URIs to add. A maximum of 100 tracks can be added in one request.
* `Accept` - _optional_ - It is used to set specified media type.

### [Reorder or replace a Playlist's Tracks](https://developer.spotify.com/web-api/reorder-playlists-tracks/)

#### Input Parameters
* `user_id` - _required_ - The user's Spotify user ID.
* `playlist_id` - _required_ - The Spotify playlist ID.
* `Accept` - _optional_ - It is used to set specified media type.

## License

**flow**ground :- Telekom iPaaS / spotify-com-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
