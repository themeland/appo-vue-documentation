# Template customization


## public
I hope you have seen this template `public` folder on the downloaded package `Appo - Vue JS App Landing Page` from ThemeForest.

In this `public` folder you can see `index.html` file. This file structure is like this-

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <!--meta, title, google fonts, all css linking here-->
</head>

<body>

  <div id="app"></div>
 
 <!--all js linking here-->
</body>

</html>
```

All HTML content will be load into this `div`:
```html
<div id="app"></div>
```


## entry points

##### main.js
Template `main.js` structure looks like this-
```js
import Vue from 'vue'
import App from './App.vue'
import router from './router'

Vue.config.productionTip = false

new Vue({
  router,
  render: h => h(App),
}).$mount('#app')

```

##### app.vue
Template `app.vue` structure looks like this-
```vue
<template>
  <div id="app">
    <router-view></router-view>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style>

</style>

```


## themes

`themes` folder included on `src` folder. You can check our folder structure on `src` folder menu.
This is `theme` folder structure-
```text
|-- themes
    |-- theme-one.vue ( default theme)
    |-- theme-two.vue ( demo theme 2)
    .....
    |-- theme-nine.vue ( demo theme 9 )
```

`theme` folder contains all of our 9 demos.


## routes
In `router` folder we used `index.js`. Where we linked all the route for our all theme. For routing we used vue-router.

Routes: `router/index.js`

```js
import Vue from 'vue'
import Router from 'vue-router'
import ThemeOne from '@/themes/theme-one'
import ThemeTwo from '@/themes/theme-two'
import ThemeThree from '@/themes/theme-three'
import ThemeFour from '@/themes/theme-four'
import ThemeFive from '@/themes/theme-five'
import ThemeSix from '@/themes/theme-six'
import ThemeSeven from '@/themes/theme-seven'
import ThemeEight from '@/themes/theme-eight'
import ThemeNine from '@/themes/theme-nine'
import About from '@/components/InnerPages/About/About'
import Pricing from '@/components/InnerPages/Pricing/Pricing'
import Reviews from '@/components/InnerPages/Reviews/Reviews'
import Faq from '@/components/InnerPages/Faq/Faq'
import Login from '@/components/Accounts/Login/Login'
import Reset from '@/components/Accounts/Reset/Reset'
import Signup from '@/components/Accounts/Signup/Signup'
import Download from '@/components/InnerPages/Download/Download'
import ThankYou from '@/components/InnerPages/ThankYou/ThankYou'
import Newsletter from '@/components/InnerPages/Newsletter/Newsletter'
import ErrorOne from '@/components/InnerPages/Error/ErrorOne/ErrorOne'
import ErrorTwo from '@/components/InnerPages/Error/ErrorTwo/ErrorTwo'
import Contact from '@/components/InnerPages/Contact/Contact'
import Maintenance from '@/components/InnerPages/Maintenance/Maintenance'
import ComingSoon from '@/components/InnerPages/ComingSoon/ComingSoon'
import BlogTwoColumn from '@/components/Blogs/BlogTwoColumn/BlogTwoColumn'
import BlogThreeColumn from '@/components/Blogs/BlogThreeColumn/BlogThreeColumn'
import BlogLeftSidebar from '@/components/Blogs/BlogLeftSidebar/BlogLeftSidebar'
import BlogRightSidebar from '@/components/Blogs/BlogRightSidebar/BlogRightSidebar'
import BlogDetailsLeftSidebar from '@/components/Blogs/BlogDetailsLeftSidebar/BlogDetailsLeftSidebar'
import BlogDetailsRightSidebar from '@/components/Blogs/BlogDetailsRightSidebar/BlogDetailsRightSidebar'

Vue.use(Router)

export default new Router({
  mode: 'history',
  routes: [
    {
      path: '/',
      name: 'ThemeOne',
      component: ThemeOne
    },
    {
      path: '/theme-two',
      name: 'ThemeTwo',
      component: ThemeTwo
    },
    {
      path: '/theme-three',
      name: 'ThemeThree',
      component: ThemeThree
    },
    {
      path: '/theme-four',
      name: 'ThemeFour',
      component: ThemeFour
    },
    {
      path: '/theme-five',
      name: 'ThemeFive',
      component: ThemeFive
    },
    {
      path: '/theme-six',
      name: 'ThemeSix',
      component: ThemeSix
    },
    {
      path: '/theme-seven',
      name: 'ThemeSeven',
      component: ThemeSeven
    },
    {
      path: '/theme-eight',
      name: 'ThemeEight',
      component: ThemeEight
    },
    {
      path: '/theme-nine',
      name: 'ThemeNine',
      component: ThemeNine
    },
    {
      path: '/about',
      name: 'About',
      component: About
    },
    {
      path: '/pricing',
      name: 'Pricing',
      component: Pricing
    },
    {
      path: '/reviews',
      name: 'Reviews',
      component: Reviews
    },
    {
      path: '/faq',
      name: 'Faq',
      component: Faq
    },
    {
      path: '/login',
      name: 'Login',
      component: Login
    },
    {
      path: '/reset',
      name: 'Reset',
      component: Reset
    },
    {
      path: '/signup',
      name: 'Signup',
      component: Signup
    },
    {
      path: '/download',
      name: 'Download',
      component: Download
    },
    {
      path: '/thank-you',
      name: 'ThankYou',
      component: ThankYou
    },
    {
      path: '/newsletter',
      name: 'Newsletter',
      component: Newsletter
    },
    {
      path: '/error-one',
      name: 'ErrorOne',
      component: ErrorOne
    },
    {
      path: '/error-two',
      name: 'ErrorTwo',
      component: ErrorTwo
    },
    {
      path: '/contact',
      name: 'Contact',
      component: Contact
    },
    {
      path: '/maintenance',
      name: 'Maintenance',
      component: Maintenance
    },
    {
      path: '/coming-soon',
      name: 'ComingSoon',
      component: ComingSoon
    },
    {
      path: '/blog-two-column',
      name: 'BlogTwoColumn',
      component: BlogTwoColumn
    },
    {
      path: '/blog-three-column',
      name: 'BlogThreeColumn',
      component: BlogThreeColumn
    },
    {
      path: '/blog-left-sidebar',
      name: 'BlogLeftSidebar',
      component: BlogLeftSidebar
    },
    {
      path: '/blog-right-sidebar',
      name: 'BlogRightSidebar',
      component: BlogRightSidebar
    },
    {
      path: '/blog-details-left-sidebar',
      name: 'BlogDetailsLeftSidebar',
      component: BlogDetailsLeftSidebar
    },
    {
      path: '/blog-details-right-sidebar',
      name: 'BlogDetailsRightSidebar',
      component: BlogDetailsRightSidebar
    }
  ]
})

```


## components
Under `components` folder we wrote all of our components individually. 
We have written these components to make the developer’s life easy. 
By using these basic components, For example in our components directory there is `Header`, `Hero` , `Footer` folder where we wrote our different styled component. For example `Hero` component-

### Component folder structure
```text
|-- components
    ....
    |-- Hero ( hero component folder )
        - HeroOne.vue ( main demo hero section )
        - HeroTwo.vue ( demo two hero section )
        ...... ( and other )
        
    |-- Contact ( contact folder )
        - Contact.vue
    .
    ..
    ...    
```

### Contact component
`Contact/Contact.vue`
```vue
<template>
    <section id="contact" class="contact-area bg-gray ptb_100">
        <div class="container">
            <div class="row justify-content-center">
                <div class="col-12 col-md-10 col-lg-6">
                    <!-- Section Heading -->
                    <div class="section-heading text-center">
                        <h2 class="text-capitalize">Stay Tuned</h2>
                        <p class="d-none d-sm-block mt-4">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Laborum obcaecati dignissimos quae quo ad iste ipsum officiis deleniti asperiores sit.</p>
                        <p class="d-block d-sm-none mt-4">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Laborum obcaecati.</p>
                    </div>
                </div>
            </div>
            <div class="row">
                <div class="col-12">
                    <!-- Contact Box -->
                    <div class="contact-box text-center">
                        <!-- Contact Form -->
                        <form id="contact-form" method="POST" action="assets/php/mail.php">
                            <div class="row">
                                <div class="col-12 col-md-6">
                                    <div class="form-group">
                                        <input type="text" class="form-control" name="name" placeholder="Name" required="required">
                                    </div>
                                    <div class="form-group">
                                        <input type="email" class="form-control" name="email" placeholder="Email" required="required">
                                    </div>
                                    <div class="form-group">
                                        <input type="text" class="form-control" name="subject" placeholder="Subject" required="required">
                                    </div>
                                </div>
                                <div class="col-12 col-md-6">
                                    <div class="form-group">
                                        <textarea class="form-control" name="message" placeholder="Message" required="required"></textarea>
                                    </div>
                                </div>
                                <div class="col-12">
                                    <button class="btn btn-bordered mt-3 mt-sm-4" type="submit">Send Message</button>
                                </div>
                            </div>
                        </form>
                        <p class="form-message"></p>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {

}
</script>

<style>

</style>
```

## theme installtion
To install the theme you have to install [vue](https://cli.vuejs.org/) than go to the theme root dir where `package.json` located and use
```bash
npm install
```
it will install the packages.

After install process now you can run local server- local server port is 'http://localhost:8080' For developement start use
```bash
npm run serve
```
## Build your theme
```bash
npm run build
```

## For deployment -- static server
First install
```bash
npm install -g serve
serve -s build
```
If you want to know more about static deployment please visit [Create vue app deployment](https://cli.vuejs.org/guide/deployment)

Enjoy your theme :)
