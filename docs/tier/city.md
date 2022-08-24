## `city` Tier

----

* <request type="list"></request> [/api/:version/city](#apiversioncity)
* <request type="show"></request> [/api/:version/city/:uuid](#-apiversioncityuuid)
* <request type="create"></request> [/api/:version/city](#-apiversioncity)
* <request type="update"></request> [/api/:version/city/:uuid](#-apiversioncityuuid-1)
* <request type="delete"></request> [/api/:version/city/:uuid](#-apiversioncityuuid-2)
* <request type="grid-image-upload"></request> [/api/:version/city/:uuid/grid-image/upload](#-apiversioncityuuidgrid-imageupload)
* <request type="photo-upload"></request> [/api/:version/city/:uuid/photo/upload](#-apiversioncityuuidphotoupload)

----

### <request type="list"></request>/api/:version/city

Returns list of records.

<!-- tabs:start -->

#### **Auth**

- Requires: `AuthToken`
- Permission: `api.city.index`

#### **Response**

> 200

Returns JSON as array of objects.

```json
[
  {...},
  {...},
]
```

Each object is similar to:

[_show.md](../_response/city/_show.md ':include')

<!-- tabs:end -->


### <request type="show"></request> /api/:version/city/:uuid

Returns a single record.

<!-- tabs:start -->

#### **Auth**

- Requires: `AuthToken`
- Permission: `api.city.show`

#### **Response**

> 200

[_show.md](../_response/city/_show.md ':include')

<!-- tabs:end -->


### <request type="create"></request> /api/:version/city

Create a new record.

<!-- tabs:start -->

#### **Parameters**

[_generic.md](../_parameter/city/_generic.md ':include')

#### **Auth**

- Requires: `AuthToken`
- Permission: `api.city.create`

#### **Request**

```json
{
  "name": "New record name"
}
```

#### **Response**

> 201

[_show.md](../_response/city/_show.md ':include')

<!-- tabs:end -->


### <request type="update"></request> /api/:version/city/:uuid

Updates a new record.

<!-- tabs:start -->

#### **Parameters**

[parameters.md](../_parameter/city/_generic.md ':include')

#### **Auth**

- Requires: `AuthToken`
- Permission: `api.city.update`

#### **Request**

```json
{
  "name": "Updated name",
}
```

#### **Response**

> 200

[_show.md](../_response/city/_show.md ':include')

<!-- tabs:end -->


### <request type="delete"></request> /api/:version/city/:uuid

Deletes a new record.

<!-- tabs:start -->

#### **Auth**

- Requires: `AuthToken`
- Permission: `api.city.delete`

#### **Response**

> 200

[_show.md](../_response/city/_show.md ':include')

If resource is `soft-deletable` two additional property will return in json object:

```json
{
  ...
  "deleted_at": "2022-08-22 06:58:40",
  "deleted_by": "xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx"
}
```

<!-- tabs:end -->


### <request type="grid image upload"></request> /api/:version/city/:uuid/grid-image/upload

Uploads a grid image for the record.

<!-- tabs:start -->


#### **Parameters**

[_generic.md](../_parameter/media/_generic.md ':include')

#### **Auth**

- Requires: `AuthToken`
- Permission: `api.city.grid_image_upload`

#### **Request**

[_grid_image_upload.md](../_request/media/_grid_image_upload.md ':include')

#### **Response**

> 201

[_uploaded_grid_image.md](../_response/media/_uploaded_grid_image.md ':include')

<!-- tabs:end -->


### <request type="photo upload"></request> /api/:version/city/:uuid/photo/upload

Uploads a photo for the record.

<!-- tabs:start -->


#### **Parameters**

[_generic.md](../_parameter/media/_generic.md ':include')

#### **Auth**

- Requires: `AuthToken`
- Permission: `api.city.photo_upload`

#### **Request**

[_photo_upload.md](../_request/media/_photo_upload.md ':include')

#### **Response**

> 201

[response_profile_picture.md](../_response/media/_uploaded_photo.md ':include')

<!-- tabs:end -->
