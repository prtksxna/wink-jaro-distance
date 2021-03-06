
# wink-jaro-distance

> An Implementation of [Jaro Distance](https://en.wikipedia.org/wiki/Jaro%E2%80%93Winkler_distance#Jaro_distance) Algorithm by Matthew A. Jaro

### [![Build Status](https://api.travis-ci.org/decisively/wink-jaro-distance.svg?branch=master)](https://travis-ci.org/decisively/wink-jaro-distance) [![Coverage Status](https://coveralls.io/repos/github/decisively/wink-jaro-distance/badge.svg?branch=master)](https://coveralls.io/github/decisively/wink-jaro-distance?branch=master)

<img align="right" src="https://decisively.github.io/wink-logos/logo-title.png" width="100px" >

**wink-jaro-distance** is a part of **[wink](https://www.npmjs.com/~sanjaya)**, which is a family of Machine Learning NPM packages. They consist of simple and/or higher order functions that can be combined with NodeJS `stream` and `child processes` to create recipes for analytics driven business solutions.

It is a name matching algorithm that is often used during de-duplication. It computes the similarity and distance between two strings by taking into account the insertions, deletions and transpositions.

## Installation
Use **[npm](https://www.npmjs.com/package/wink-jaro-distance)** to install:
```
npm install wink-jaro-distance --save
```


## Usage
```javascript

// Load Jaro Distance Function
var jaro = require( 'wink-jaro-distance' );

console.log( jaro( 'father', 'farther') );
// -> { distance: 0.04761904761904756, similarity: 0.9523809523809524 }

console.log( jaro( 'Angelina', 'Angelica') );
// -> { distance: 0.08333333333333337,  similarity: 0.9166666666666666 }

console.log( jaro( 'Flikr', 'Flicker' ) );
// -> { distance: 0.09523809523809523, similarity: 0.9047619047619048 }

console.log( jaro( 'abcdef', 'fedcba'  ) );
// -> { distance: 0.6111111111111112, similarity: 0.38888888888888884 }

```

## Need Help?
If you spot a bug and the same has not yet been reported, raise a new [issue](https://github.com/decisively/wink-jaro-distance/issues) or consider fixing it and sending a pull request.


## Copyright & License
**wink-jaro-distance** is copyright 2017 GRAYPE Systems Private Limited.

It is licensed under the under the terms of the GNU Affero General Public License as published by the Free
Software Foundation, version 3 of the License.
