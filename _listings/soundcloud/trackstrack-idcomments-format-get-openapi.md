---
swagger: "2.0"
x-collection-name: SoundCloud
x-complete: 0
info:
  title: Sound Cloud Get Tracks Track Comments. Format
  description: Returns comments of a track by track id
  version: 1.0.0
host: api.soundcloud.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /tracks/{track_id}.json:
    get:
      summary: Get Tracks Track
      description: Returns a track by track id
      operationId: getTracksTrack.json
      x-api-path-slug: trackstrack-id-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Tracks
      - Track
    put:
      summary: Put Tracks Track
      description: Updates a given track
      operationId: putTracksTrack.json
      x-api-path-slug: trackstrack-id-json-put
      responses:
        200:
          description: OK
      tags:
      - Tracks
      - Track
    delete:
      summary: Delete Tracks Track
      description: Deletes a given track
      operationId: deleteTracksTrack.json
      x-api-path-slug: trackstrack-id-json-delete
      responses:
        200:
          description: OK
      tags:
      - Tracks
      - Track
  /tracks/{track_id}/comments.json:
    get:
      summary: Get Tracks Track Comments
      description: Returns comments of a track by track id
      operationId: getTracksTrackComments.json
      x-api-path-slug: trackstrack-idcomments-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Tracks
      - Track
      - Comments
    post:
      summary: Post Tracks Track Comments
      description: Posts a comments to a track by track id
      operationId: postTracksTrackComments.json
      x-api-path-slug: trackstrack-idcomments-json-post
      responses:
        200:
          description: OK
      tags:
      - Tracks
      - Track
      - Comments
  /tracks/{track_id}/permissions.json:
    get:
      summary: Get Tracks Track Permissions
      description: Returns all users with permission for a track by track id
      operationId: getTracksTrackPermissions.json
      x-api-path-slug: trackstrack-idpermissions-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Tracks
      - Track
      - Permissions
    put:
      summary: Put Tracks Track Permissions
      description: Updates the list of permitted users for a track by track id
      operationId: putTracksTrackPermissions.json
      x-api-path-slug: trackstrack-idpermissions-json-put
      responses:
        200:
          description: OK
      tags:
      - Tracks
      - Track
      - Permissions
  /tracks/{track_id}/secret-token.json:
    get:
      summary: Get Tracks Track Secret Token
      description: Returns the secret token for a track by track id. This resource
        can only be used by the track owner.
      operationId: getTracksTrackSecretToken.json
      x-api-path-slug: trackstrack-idsecrettoken-json-get
      responses:
        200:
          description: OK
      tags:
      - Tracks
      - Track
      - Secret
      - Token
    put:
      summary: Put Tracks Track Secret Token
      description: |-
        Resets the secret token for a track by track id. The secret token can not be specified but will be randomly chosen on
                  the server and returned. This resource can only be used by the track owner.
      operationId: putTracksTrackSecretToken.json
      x-api-path-slug: trackstrack-idsecrettoken-json-put
      responses:
        200:
          description: OK
      tags:
      - Tracks
      - Track
      - Secret
      - Token
  /users/{user_id}/favorites/{track_id}.json:
    put:
      summary: Put Users Favorites Track
      description: Adds the given track to the given user's list of favorites.
      operationId: putUsersUserFavoritesTrack.json
      x-api-path-slug: usersuser-idfavoritestrack-id-json-put
      responses:
        200:
          description: OK
      tags:
      - Users
      - Favorites
      - Track
    delete:
      summary: Delete Users Favorites Track
      description: Deletes the given track from the given user's list of favorites.
      operationId: deleteUsersUserFavoritesTrack.json
      x-api-path-slug: usersuser-idfavoritestrack-id-json-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - Favorites
      - Track
  /me/favorites/{track_id}.json:
    put:
      summary: Put Me Favorites Track
      description: Adds the given track to the logged-in user's list of favorites.
      operationId: putMeFavoritesTrack.json
      x-api-path-slug: mefavoritestrack-id-json-put
      responses:
        200:
          description: OK
      tags:
      - Me
      - Favorites
      - Track
    delete:
      summary: Delete Me Favorites Track
      description: Deletes the given track from the logged-in user's list of favorites.
      operationId: deleteMeFavoritesTrack.json
      x-api-path-slug: mefavoritestrack-id-json-delete
      responses:
        200:
          description: OK
      tags:
      - Me
      - Favorites
      - Track
  /tracks/{track_id}.{format}:
    get:
      summary: Get Tracks Track . Format
      description: Returns a track by track id
      operationId: getTracksTrack.Format
      x-api-path-slug: trackstrack-id-format-get
      parameters:
      - in: query
        name: consumer_key
        description: Access, host, upload, and comment on audio
      - in: path
        name: track_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Tracks
      - Track
      - ""
      - ""
      - Format
    put:
      summary: Put Tracks Track . Format
      description: Put tracks track . format.
      operationId: putTracksTrack.Format
      x-api-path-slug: trackstrack-id-format-put
      parameters:
      - in: query
        name: asset_data
        description: Access, host, upload, and comment on audio
      - in: query
        name: title
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Tracks
      - Track
      - ""
      - ""
      - Format
    delete:
      summary: Delete Tracks Track . Format
      description: Delete tracks track . format.
      operationId: deleteTracksTrack.Format
      x-api-path-slug: trackstrack-id-format-delete
      parameters:
      - in: path
        name: track_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Tracks
      - Track
      - ""
      - ""
      - Format
  /tracks/{track_id}/comments.{format}:
    get:
      summary: Get Tracks Track Comments. Format
      description: Returns comments of a track by track id
      operationId: getTracksTrackComments.Format
      x-api-path-slug: trackstrack-idcomments-format-get
      parameters:
      - in: query
        name: consumer_key
        description: Access, host, upload, and comment on audio
      - in: path
        name: track_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Tracks
      - Track
      - Comments
      - ""
      - Format
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---