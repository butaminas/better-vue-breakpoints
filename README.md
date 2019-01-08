# better-vue-breakpoints

[![npm](https://img.shields.io/npm/v/better-vue-breakpoints.svg)](https://www.npmjs.com/package/list-of-currencies)


Based on https://github.com/cb109/vue-md-breakpoint, this package lets you use predefined breakpoints instead of hardcoded material design breakpoints.
Bootstrap breakpoints are set by default.

## Installation
```bash
$ npm i better-vue-breakpoints
$ yarn better-vue-breakpoints
```


## Usage

You can either import it into your component or use it in your app.js to make it work globally:
    
##### Declare use in your App / Component:
    import Vue from 'vue';
    import breakpoint from 'better-vue-breakpoints';

    Vue.use(breakpoint) // Default breakpoints (Bootstrap)
    
    // if you want to use custom breakpoints:
    Vue.use(breakpoint, {
      xs: 576,
      sm: 768,
      md: 992,
      lg: 1200,
      xl: 1920,
    })
##### Use in your template:
    <div v-if="$breakpoint.smAndUp"></div>
##### Or anywhere else:
    awesomeMethod() {
        if (this.$breakpoint.smAndUp") {
            return "Awesome"
        }
    }

## API

- `$breakpoint.name`
- `$breakpoint.xsOnly`
- `$breakpoint.smOnly`
- `$breakpoint.smAndDown`
- `$breakpoint.smAndUp`
- `$breakpoint.mdOnly`
- `$breakpoint.mdAndDown`
- `$breakpoint.mdAndUp`
- `$breakpoint.lgOnly`
- `$breakpoint.lgAndDown`
- `$breakpoint.lgAndUp`
- `$breakpoint.xlOnly`
- `$breakpoint.width`
- `$breakpoint.height`
