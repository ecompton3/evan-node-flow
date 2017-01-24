Node Flow
=========

This assumes the starting point is a user signed into Bluemix

Explore
-------

* Dropped into the dashboard, I select Create App as it's the only way it seems to make an app.
* On the Catalog page I see four different Node.js boilerplates
  - As a new Node developer I have no idea what LoopBack or StrongLoop Arc are, clicking on them provides little info, I avoid
  - The Personality Insights one seems interesting but I have no use for that in my app so I also avoid it
  - I have no idea how Node-RED compares to Node, again the description is unhelpful so I avoid
* Ultimately I decide to stick with the generic Node runtime
  - Oddly this is called SDK for Node.JS, this doesn't make much sense at all because this is Node not an SDK _for_ node
Evaluate
--------
* With the Node runtime found, I can now download and play with the code and see what a simple deploy looks like
* Thankfully Bluemix provides me with the CLI tool and Starter code upon creating the app
  - I download and install both of these, the process is painless
* I immediately open the code in my preferred editor (VSCode) and start looking at it
  - I check the `app.js` file, it is very simple but well documented. The comments about cfenv are most helpful
  - I then check the `package.json` to see the dependencies needed for this app, I'm happy that's there's only two
  - Finally I check the Readme to see if there's anything special I need to do, happily its just a standard npm install and start
* I run the install and start commands to see it running locally, the server actually starts on a different port than what the README says,
but the terminal outputs the port so I can still easily check it.
  - As an aside, this is because of how cfenv works. For most people it should start on the same port but for me it doesnt because of how often I use it
* I check out the simple Hello World page, see its running pretty much like any other node app I've done before
* I decide to do a push to Bluemix to see what a deploy looks like, using the sample commands on the BMX site
* The push was very easy, but the terminal outputs that its downloading a bunch of unrelated buildpacks, this confuses me
* The push actually fails, I run the log command it gives me, as far as I can tell the platform just crashed, this does not fill me with confidence
* I try a second push, it also fails, as a normal user I'd give up by now
* Third try finally works, I go to the URL the terminal prints out, I can see it running. I now feel confident to try making an actual app

Embrace
------

* At this point all development is done locally, I'm assuming no services at this point, occassionally there might be pushes up to test out any API's made
* I now have a basic app and want to automate my build process, in the Getting Started section there is a card about Continous Delivery, I investigate
* 

Extend
------

Expand
------