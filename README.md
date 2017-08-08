# vue-douban
> 豆vue-douban

## Features

- Vue + vue-router + vuex + vue-resource working together
- Vuex divide store into modules
- Modern JavaScript syntax with ES6
- vue-cli webpack template
- Single-file Vue Components
- API request seperated
- Real remote API and some mock data
- eslint linter integration
- Hot-reload in development
- Css with Sass
- No third party CSS framework
- Complex and different style view logic
- Infinite loading list
- Complete search logic
- Custom components like List, Rating, Tags ...
- Authentication with JSON Web Tokens developing
- Complete login logic developing
......


## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8086
npm run dev

# build for production with minification
npm run build

```

For detailed explanation on how things work, checkout the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).

## Libraries

- [Vuex](https://vuex.vuejs.org) : Centralized State Management for Vue.js
- [Vue-router](http://router.vuejs.org/) : The official router for Vue.js
- [vue-resource](https://github.com/pagekit/vue-resource) : The HTTP client for Vue.js
- [vue-infinite-loading](https://github.com/PeachScript/vue-infinite-loading) : An infinite scroll plugin for Vue.js 1.0 & Vue.js 2.0.
- [normalize.css](https://github.com/necolas/normalize.css) :  A collection of HTML element and attribute style-normalizations

## API

- Basic URI : `https://api.douban.com/V2/`
- Online activities
 - Activities list : `/event/list?loc=108288&count=&start=`
 - Single activitie info : `/event/id`
- Movie
 - In theaters : `/movie/in_theaters?count=`
 - Coming soon : `/movie/coming_soon?count=`
 - Top 250 : `/movie/top250?count=`
 - Single movie info : `/movie/subject/id`
- Book
 - Search some books : `/book/search?q=&count=`
 - Single book info : `/book/id`
- Search
 - Search books : `/book/search?q=`
 - Search movie : `/movie/search?q=`
 - Search music : `/music/search?q=`
- Login
 - In development

For detailed explanation, checkout the [douban api](https://developers.douban.com/wiki/?title=api_v2)

## File Structure
```
.
├── build
│   ├── build.js
│   ├── check-versions.js
│   ├── dev-client.js
│   ├── dev-server.js
│   ├── utils.js
│   ├── vue-loader.conf.js
│   ├── webpack.base.conf.js
│   ├── webpack.dev.conf.js
│   └── webpack.prod.conf.js
├── config
│   ├── dev.env.js
│   ├── index.js
│   └── prod.env.js
├── index.html
├── LICENSE
├── package.json
├── README.md
├── src
│   ├── App.vue
│   ├── assets
│   │   ├── book_zw.jpg
│   │   ├── douban-app-logo.png
│   │   └── promotion_bg.jpg
│   ├── components
│   │   ├── Banner.vue
│   │   ├── Card.vue
│   │   ├── DownloadApp.vue
│   │   ├── Group.vue
│   │   ├── HeaderBar.vue
│   │   ├── List.vue
│   │   ├── Rating.vue
│   │   ├── Scroller.vue
│   │   ├── SubjectMark.vue
│   │   ├── SubNav.vue
│   │   ├── Tags.vue
│   │   └── Types.vue
│   ├── main.js
│   ├── router
│   │   └── index.js
│   ├── store
│   │   ├── index.js
│   │   └── modules
│   │       ├── activities.js
│   │       ├── book.js
│   │       ├── group.js
│   │       ├── movie.js
│   │       ├── search.js
│   │       └── subject.js
│   └── views
│       ├── BookView.vue
│       ├── DetailView.vue
│       ├── GroupView.vue
│       ├── HomeView.vue
│       ├── MovieView.vue
│       ├── PagesView.vue
│       ├── SearchView.vue
│       ├── StatusView.vue
│       ├── SubjectView.vue
│       └── TalionView.vue
└── static
    └── logo.png
```

基于vue仿豆瓣
