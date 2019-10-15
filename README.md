# Profile Site for Takuma Osada 
![GitHub release (latest by date)](https://img.shields.io/github/v/release/takumaosada/ostk_profile)
[![Actions Status](https://github.com/takumaosada/ostk_profile/workflows/Deploy/badge.svg)](https://github.com/takumaosada/ostk_profile/actions)
[![Twitter](https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Fgithub.com%2Ftakumaosada%2Fostk_profile)](https://twitter.com/intent/tweet?text=Wow:&url=https%3A%2F%2Fgithub.com%2Ftakumaosada%2Fostk_profile)

## Detail for Takuma Osada
Please check: https://github.com/takumaosada/profile

## Installation & Commands

### Setup packages
```
npm install
```
Please install `npm` command if you are not ready for this.

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```

### Initialize Firebase
```
firebase init
```

### Deploy
after `npm run build` successfully passed, run 
```
firebase deploy
```

Also, as you can see Github Actions Tab in this repository,  
it automatically try to deploy with Firebase Hosting when pull request successfully merged.  
You can check [here](https://github.com/takumaosada/ostk_profile/blob/master/.github/workflows/deploy.yml) for more detail.

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
