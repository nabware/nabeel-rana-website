# Nabeel Rana Website

## Todo

- [x] Add navbar
- [x] Add landing section with photo
- [x] Add About Me section with PDF resume
- [x] Add contact info
- [x] Publish to internet

## Deploy

```
sam build
sam deploy --guided
aws s3 sync ./src s3://BUCKET-NAME --delete
aws cloudfront create-invalidation --distribution-id DISTRIBUTION-ID --paths "/*"
```