# Image Capture Repo

See S3 info [here](./docs/S3.md)

## Getting Screenshots

Start the local server with:
```
cd captures
npm i
npm run start
```

Navigate to `localhost:8080` and select places to screenshot with `N` and `Return`

Metadata will be saved to working-data

Mass-export screenshots with:
```
npm run export
```

## Exporting Posters

Screenshots saved in '/working-data' will be converted to posters and then saved back into '/working-data/exports'

```
cd designing
python runner.py
```


## S3 interfacing

Interface with the cloud to store and retrieve files

```
cd cloud
python sync.py
```
