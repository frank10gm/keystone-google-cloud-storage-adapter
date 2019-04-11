# Google Cloud Storage adapter for KeystoneJS

This adapter is designed to use it in KeystoneJS File field.

## Usage

Configure the storage adapter:

```js
var storage = new keystone.Storage({
  adapter: require('keystone-storage-adapter-cloud-storage'),
  cloudStorage: {
    keyFilename: 'gcloud_auth.json',
    path: 'uploads/',
    bucket: 'the-bucket-name',
    uploadOptions: {
      public: true
    }
  },
  schema: {
    url: true,
  },
});
```