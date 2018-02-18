ipfsearch-index generates index and inverted index for use by ipfsearch-webapp.

# Usage
```
import * as ipfsearch from "ipfsearch-indexlib"
let indexer = new ipfsearch.Indexer()
indexer.addToIndex(new ipfsearch.Document("Python","A great, nice programming language. Super user-friendly."))
indexer.addToIndex(new ipfsearch.Document("Javascript","A language that was hacked together in 14 days and ECMA is trying to make it better. Still feels hacked together tho"))
//add more docs...


indexer.persist("assets/sortedindex.inx", "assets/index.inx","authors name","index name")
```

# Building

Clone this repo and run:

```
$ npm install
$ node_modules/typescript/bin/tsc -p tsconfig.json
```

# Test index
The meta.json for the files has been generated and saved to ipfs at QmUFVKRPGsGUziEydsic91GfuDzJTjXdoxSiv9dHjutv1g. It references another ipfs directory that contains the generated invinx and inx.