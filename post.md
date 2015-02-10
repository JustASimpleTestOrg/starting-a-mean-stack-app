## 1 Why a new AirPair.com?

Hi :{} I'm Jonathon, you can follow me on Twitter at [@hackerpreneur](http://twitter.com/hackerpreneur) to keep tabs on my 90-day vision quest to show how powerful AirPairing can be. AirPair is my 3rd startup, and the new AirPair.com code base - which I started today - is the 6th code base I've started from scratch in my startup career. I spent years learning and getting stuck, **so I set out to create a service that would stop people from giving up because of technology** before they could watch their business assumptions play out. We've been lucky to collect a great team, go through YCombinator, and get backing from some amazing Silicon Valley investors. We're excited to be leading our space and to build a next-generation experience that will help us continue as the market leader with the highest quality experts and best customer support.

<br />
<iframe width="640" height="360" src="//www.youtube-nocookie.com/embed/qlOAbrvjMBo" frameborder="0" allowfullscreen>
</iframe>
<br /><br />
So far, using AirPair has helped me overcome technology challenges in dribs and drabs. But our ultimate vision of on-demand elastic knowledge has not yet been realized: we see a world where AirPairing makes up as much as 5% of human resources and multiplies software team productivity. 

I think the following barriers have gotten in the way of that vision. Now, we're ready to overcome them with a new site and the experience of building it while eating our own dog food.

### 1.1 Cost

I've never had a budget for AirPairing more than 5% of the time. Truth is, AirPair only works when there's a project with a proper development budget. Getting the best people to work with you isn't cheap. You could work with cheaper competitors, but if you are serious about multiplying your productivity, you need to invest in quality help -- like you do with your full-time developers. Now that we have funding, I'm going to use it and show you my spend through the next 90 days.

### 1.2 Friction

The AirPair experience needs to be 10x faster at getting you help. The current AirPair site is an MVP we built 18 months ago; I'm quite proud of it, and will blog about my philosophy *"Release Often, Release Dirty"* another time. But we're ready to give you that order of magnitude improvement on expert response time and matching quality. <a href="http://twitter.com/home?status=@hackerprenuer I would love to be a beta tester for the new ap" target="_blank">Tweet at me</a> if you'd like to be a beta tester. We'll be releasing builds every week for community feedback and bug squashing help.

### 1.3 Dedication

AirPairing is about consuming knowledge at warp speed **while** you see your project come to life. Learning is tiring, and AirPairing properly involves buying in up front with as much dedication as you would when studying a new course. For the last 18 months, I've been context switching between development, marketing, and investor relations. This is the first time I've dedicated 3 straight months of focus to code. I'm switching from Backbone.js and ready to become an AngularJS ninja.


## 2 Choosing MEAN Stack 
Mean = [`MongoDB, ExpressJS, AngularJS & NodeJS`]

<img src="//s3.amazonaws.com/media-p.slid.es/uploads/jbpionnier/images/196683/mean_small_vertical.png" style="margin:40px 40px 30px 0px;float:left" />

Having used `MongoDB` for a year, I've grown to like document-driven databases. It's a fast way to develop. I like nesting documents and avoiding joins. It leads to less code, fewer database trips and HTTP requests. There are problems and overhead with replicated data, which may lead us to switch to SQL eventually, but for now Mongo suits our product and development styles really well.

I'm not one for religious debates on which languages to use. I like technologies that `(a)` help you get a lot of shit done quickly and `(b)` lots of people know and are easy to hire for. I came from .NET, where I used to write in c# on the server and various JavaScript on the client side. Full-stack JavaScript with `NodeJS` and `ExpressJS` meant I didn't need to learn a new language and could become doubly proficient in one.

I really love `Backbone.js`, but having tried to teach it to a few people and watch them struggle before grasping `AngularJS` way quicker, I've got a feeling its going to be 3-4 times easier to learn and build on. It's also the most widely adopted and quickly growing front-end framework. I've seen that not only through the notorious graphs of people searching for AngularJS, but first hand with how many requests we get for help with Angular.

## 3 Gulp as an Application Assembler

<img src="https://raw2.github.com/gulpjs/artwork/master/gulp-2x.png" style="margin:60px 20px 15% 20px;width:160px;float:right" />

The last version of AirPair.com was built using <a href="http://brunch.io/" target="_blank">`brunch.io`</a> as the application assembler to compile, combine, concat and minify JavaScript (coffeescript), CSS (sass) and watch / auto rebuild changes while developing. I really liked it, but a few engineers I worked with didn't. I think the main thing they were annoyed at was needing to restart the brunch server when making server-side changes as it only client-side automatically.

I knew about <a href="//gruntjs.com/" target="_blank">`grunt`</a> as an alternative to brunch, but I'd actually not heard of <a href="http://gulpjs.com/" target="_blank">`gulp`</a> - the latest and greatest. Thanks to a quick chat in my AirPair Angular War Room with my support experts including Matias Nemila (AngularJS Core Team), Uri Shaked (AngularJS Google Developer Expert) and Ari Lerner (Author of ng-book and ng-newsletter), I was quickly pointed in the optimal direction without needing to spend hours on research.

The main advantages of gulp are code-based configuration vs declarative and streaming (faster) builds. This <a href="http://markdalgleish.github.io/presentation-build-wars-gulp-vs-grunt/" target="_blank">awesome Grunt vs Gulp slide deck</a> by Mark Dalgleish help me appreciate the differences quickly.

### 3.1 nodemon
`nodemon` is a daemon that watches the JavaScript files in your node app and restarts the node server on any changes. Uri and I installed `gulp-nodemon` in minutes so that the annoyance of manually restarting the node server in my old workflow was gone. I really like that I don't need multiple terminals and multiple commands, everything is taken care of by gulp.

### 3.2 Less
I ended up opting for Less because you don't need ruby or c++ to compile. With `gulp-less` we got LESS to CSS compilation down relatively quickly, though we got caught on a stylesheet link tag without a `text/css` attribute that held us up for a few minutes.

###3.3 LiveReload
LiveReload is a mechanism to auto-refresh the browser when a change occurs so you don't have to manually hit refresh. It's particularly nice for CSS editing. I would have fiddled setting this up for quite a while on my own, but Uri knew what he was doing and guided me through setting up both `gulp-livereload` and `connect-livereload` on the node side. I love knocking things out as if I've done it a hundred times before.

##4 Summary
I'm excited to accomplish a lot in 3 months with the help of AirPair experts on tap. In our first hour of MEAN stack development, Uri and I set up Gulp to wrap nodemon for automatic server-side code reloads, compiling of Less, and browser LiveReload to see client-side changes appear automatically and instantly. This is already a really nice improvement on my previous work flow, and I feel I'm already coding 10% faster for the rest of the project onwards.