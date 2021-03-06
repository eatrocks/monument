### - 1.4.6 *3/17/2015, 7:06:52 AM*

  - Merge pull request #83 from eatrocks/feature/queryparamarrays
  - add util to handle array[] conventions with request parameters


### - 1.4.5 *3/11/2015, 12:04:26 PM*

  - Merge pull request #81 from ansble/bug/headers
  - expanded tests to include the other areas
  - added tests for getCompression and rolled all the utils into a utils package. cleaner... better. also cleaned the getCompression function out of the routes/index.js file so that it is independent.


### - 1.4.4 *3/9/2015, 4:35:02 PM*

  - Merge pull request #77 from ansble/e3-harelbeke
  - Merge pull request #76 from ansble/feature/in-place-tests
  - added support for inplace tests in routes which is nice


### - 1.4.3 *3/6/2015, 10:20:23 PM*

  - Merge pull request #74 from uniqname/feature/dotjs-config
  - dotjs configs


### - 1.4.2 *3/3/2015, 8:30:35 PM*

  - Merge pull request #72 from ansble/e3-harelbeke
  - Merge pull request #71 from ansble/bug/send
  - fixed the issue with temlpates and strings, seems to be working now
  - Merge pull request #70 from ansble/feature/trail-slash
  - wildcard routes are now trailing slash independent
  - renamed the function that matches simple routes to make it's purpose more clear
  - fixed the simple route matching for traliing slash... now onto the wildcard routing
  - modified the trail slash check for routes.
  - fixing the build badge


### - 1.4.1 *3/3/2015, 6:36:07 AM*

  - Merge pull request #68 from ansble/e3-harelbeke
  - updated dependencies and readme.md
  - updated the readme


### - 1.4.4 *3/3/2015, 6:24:56 AM*

  - Merge pull request #67 from ansble/milan-san-remo
  - closes #66 rewrote around own event system instead of the built in one. memory use seems more reasonable and more stable


### - 1.3.4 *2/28/2015, 8:29:51 AM*

  - Merge branch 'master' of https://github.com/ansble/monument
  - Merge pull request #65 from ansble/bug/favicon.ico
  - fixing a bug that caused favicon.ico requrests to match wildcard and crash the app under some circumstances


### - 1.3.3 *2/28/2015, 8:23:04 AM*




### - 1.3.2 *2/27/2015, 2:26:21 PM*

  - Merge pull request #64 from ansble/bug/wild-card-routes
  - fixed the wild card route matching issue


### - 1.3.1 *Sat Feb 21 2015 08:59:04 GMT-0700 (MST)*

  - Merge pull request #59 from ansble/milan-san-remo
  - fixed conflicts
  - updated the readme closes #57
  - 1.2.1
  - preparing for release of v1.2.1



### - 1.3.0 *Mon Feb 16 2015 07:06:31 GMT-0700 (MST)*

  - Merge pull request #56 from ansble/milan-san-remo
  - Merge branch 'milan-san-remo' of https://github.com/ansble/monument into milan-san-remo
  - Merge branch 'feature/etag' into milan-san-remo
  - Merge branch 'master' of https://github.com/ansble/monument into milan-san-remo
  - bug before release
  - Merge pull request #55 from ansble/feature/etag
  - linting and refactored emitter to be events'
  - trying a linhub.yml file..
  - added some project config files
  - found a memory leak and fixed it... something weird with emitter.once not unbinding for some reason
  - etags working for static files now... #25 there seems to be some weird event stuff going on in the req:get:headers area though
  - compression is now a config option for real
  - added a central event manager for handling etag verification for static files and have it sort of working. works on first hit but something tries to write to the strean after it closes on 2nd hit. #25
  - etags are working with res.send now, now to handle them for static files #25
  - Merge pull request #54 from ansble/cleanup
  - clenaed up the readme.md and updated the keywords in package.json #52 and #53 respectively
  - added a line for configuring if etags are used
  - Update license.md
  - Update license.md
  - Update license.md
  - Update license.md
  - Merge branch 'milan-san-remo' of https://github.com/ansble/monument into feature/etag
  - added the etag library of choice and about ready to tackle #25
  - Merge pull request #51 from ansble/feature/compress
  - more tweaks to readme
  - stubbed tests, added more readme and made compression configurable
  - Merge pull request #49 from ansble/feature/compress
  - added v0.12 to the travis.yml
  - so much work on the gzip/deflate... opting for gzip by default. Caching the file to filesystem so that subsiquent requests are fast fast fast. this finishes the work on #26
  - added a test for the detection of the required module
  - removing the old stuff that isn't used now because this is an npm module and not a monolithic server
  - working on caching the compressed file to file system
  - rough implementation of q value calulation for accept-encoding. Probably slow and needs work... #26
  - basic compression should be working now #26
  - added rudimentary compression checking... once that is nailed then I'll add in the more advanced q value calulation
  - Merge branch 'milan-san-remo' of https://github.com/ansble/monument into milan-san-remo
  - Merge branch 'master' of https://github.com/ansble/monument into milan-san-remo
  - worked on the package.json a bit
  - Merge pull request #48 from ansble/master
  - Merge pull request #47 from ansble/feature/send
  - minor tweak to change how buffers are dealt with
  - basic version of .send is now in and working. closes #41
  - closes #44 and wraps up the required event stuff
  - revved the version on event-state which is much nicer now
  - Merge branch 'master' into feature/send
  - Merge pull request #46 from ansble/bug/query
  - fixed... the bug closes #45"
  - added the state maching state-event to monument
  - more progress on the send function. Close to singing
  - working away on the send method... almost have it cleaned up and to par
  - more work on #41 clearing out the cruft from the express code
  - added an update to the readme.md that links to the depdnency status. Also started laying out the send modules in utls folder. The express source for res.send is in there now so I can make sure my bases are covered for usage and edge cases.
  - added a bunch of badges and more badges


### - 1.2.23 *Thu Jan 29 2015 06:29:32 GMT-0700 (MST)*

  - added a bunch of badges
  - added a bunch of badges
  - Merge pull request #40 from ansble/gent-wevelgem
  - added an 0.11 test as well
  - added a travis.yml file for automated build tests
  - a little more cleanup in the parsePath function and I think we are ready to rock and roll #38
  - cleaning up the  commented out lines from #38
  - more change to go with #38 getting things much cleaner and more elegant. Revised the body handling and the parser. Much nicer now
  - revised to match the new paradigm
  - revised the route and connection modules to match the line of reasoning in #38. More functional, a little cleaner and a diversion from the standard model of other node app frameworks that modify the incoming request. Now we don't. They are added to the connection object that wraps the request and response objects. This changes how you work with the request.
  - Merge pull request #39 from ansble/feature/documentation
  - finished with documentation for the moment #11
  - more documentation on routes for #11
  - so much more documentation
  - working on the documentation on routes and contributing for #11
  - Merge pull request #37 from ansble/feature/tests-initial
  - added a lot of tests and made it big
  - reworked the gulp file to have a release task that automates all the release code. Should be awesome and much easier.
  - preparing for release of v1.1.24
  - preparing for release of v1.1.24
  - preparing for release of v1.1.24
  - getting more testing done and added some pre-work for release automation. #8
  - getting the base tests written starting with the event emitter module. also added the dependencies needed to get testing rolling. #8


