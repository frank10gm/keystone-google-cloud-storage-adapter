# Google Cloud Storage adapter for KeystoneJS

This adapter is designed to use it in KeystoneJS File field.

## Install

`npm i keystone-google-cloud-storage-adapter --save`

or

`yarn add keystone-google-cloud-storage-adapter`

## Usage

Configure the storage adapter:

```js
var storage = new keystone.Storage({
  adapter: require('keystone-google-cloud-storage-adapter'),
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