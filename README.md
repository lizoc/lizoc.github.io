[Lizoc Open Source](https://www.lizoc.com/opensource)
====================
Hey there! Our new portal for open source projects are now [Lizoc Open Source](https://www.lizoc.com/opensource). Version **2.0** here we go!!!

Now you can finally search repositories on **all our affiliated GitHub accounts**, filter by popularity stars, and see changes in real time.

<h4 align="center"> Lizoc += ♥ #OpenSource </h4>


What do you think?
------------------
A lot of work has gone into making our new portal, and we really hope you like the new experience. If you have an idea or found a bug, just 
submit [an issue](https://www.github.com/lizoc/lizoc.github.io/issues) and we'll get right on to it.

If this is your first time here, just [go explore](https://www.lizoc.com/opensource) and find something interesting to you.


Popping the Hood
----------------
Perhaps you are here to figure out how we made our portal. Our recipe includes:

- [Github Pages](http://pages.github.com) and [GitHub API](http://developer.github.com/v3)
- [VueJS](http://www.vuejs.org)
- [NodeJS](http://nodejs.org)
- [D3](http://d3js.org)

The whole thing goes somewhat like this:

<p align="center"><img src="https://raw.github.com/lizoc/lizoc.github.com/master/github_portal_schema.png" alt="Lizoc Open Source Portal Schema" /></p>

We run a [NodeJS server](https://www.github.com/lizoc/askoctocat) that aggregates data periodically from [GitHub API](http://developer.github.com). This allows us to 
consolidate the latest information on our GitHub repos, which is spread across multiple accounts, in one place. The NodeJS server also expose a simple restful API that 
allows us to query these information using plain AJAX web requests.

The frontend is a bunch of static content generated using TextScript templates (source code available [in this repo](https://www.github.com/lizoc/multihub)). When you visit 
our portal, your browser starts making AJAX requests to our NodeJS server, and creates some very cool visualization of the returned results.

Sounds interesting to you? Join our collaborators today!
