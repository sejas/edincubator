# shell
```bash
#change separator csv
tr "\t" ";" < demo.csv > demo-clean.csv
#imoprt
mongoimport -h ds155299.mlab.com:55299 -d edi-db -c sentimental -u <username> -p <password> --file demo-clean.csv --type csv --headerline
#connect
mongo ds155299.mlab.com:55299/edi-db -u <username> -p
```

# mongodb
```js
db.sentimental.find()
db.sentimental.findOne()
db.sentimental.remove({})
```
