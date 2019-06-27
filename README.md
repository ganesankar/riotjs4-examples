# Riot 4 Examples

This is a sample project using Riot 4 which you need only browser to compile.
I use all range of frameworks depend on my purpose. 
For most of my internal company projects don't require heavy lifting frameworks that requires
Node process like Vue, Angular, or React, but I also need to be avoid too basic like jQuery
in order to avoid chaotic situation.

The best part of Riot is that it compiles on the browser, and it supports all modern 
component based UI mechanism with reasonable learning curve. This is very useful for me because
I have to split tasks with other team members in different skill level.

*"Understand and stay way of cargo cult" - [Julio Biason .Net 4.0 - Things I Learnt The Hard Way (in 30 Years of Software Development)](https://blog.juliobiason.net/thoughts/things-i-learnt-the-hard-way/)*

## Stack 

1. [Bootstrap 4](https://getbootstrap.com/docs/4.0/getting-started/introduction/) and [SB Admin 2](https://startbootstrap.com/themes/sb-admin-2/) CSS Template and Design
2. [SB Admin 2](https://startbootstrap.com/themes/sb-admin-2/) - Componet based UI Library
3. [Akita 4](https://netbasal.gitbook.io/akita/) - State Management [CDN](https://www.pika.dev/packages/@datorama/akita)
4. [Axios 0.19.0](https://github.com/axios/axios) - HTTP
5. [Navigo 6](https://github.com/krasimir/navigo) - Routing

## Running

```
npm i -g live-server
```

Then

```
live-server
```

## Implementation

You can login using any credentials. All dummy data files are located under /api/ folder.
I saved external libraries under /vendor/. Although, it seems riot router and observable
will be coming out, this is my challenge to use other state management library and
router in clean way. One thing I couldn't figure out was, to create a nice directive like
```
<router route="dashboard"></router>
```
using mount api so that I can mount based on the route.

I also playing around with Akita. I implemented a breadcrumb which you can push some item, and pop
when you go back. Try to click "Friends" section of details page.

![sample.png (600×312)](https://raw.githubusercontent.com/kiichi/riotjs4-examples/master/screenshot/sample.png)


## Reference

- [MDN - Module Examples](https://github.com/mdn/js-examples/)
