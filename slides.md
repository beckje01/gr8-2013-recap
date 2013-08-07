# Agenda

* GR8US Keynote
* Gradle
* Groovy
* Grails
* Ratpack

~~~~
## Open Source and You

Peter Ledbrook

[Slides](https://github.com/sjurgemeyer/GR8ConfUS2013/blob/master/PeterLedbrook/open-source-and-you-gr8conf-us-2013.pdf)

~~
### Takeaways

* Any size contribution helps
* If you use open source help out 
* Docs are a great place to start

~~~~
## Gradle

A powerful build tool blending Ant and Maven.

~~
### Workshop

A good overview starting from the basics. There are slides and excersises to work through.

Zip of all materials available from USB Stick.

~~
### Building Grails with Gradle

* Gradle is faster than ivy at dependency resolution
* All or nothing solution
* Grails 3 will use gradle as the build system
* Doesn't currently work with Grails 2.3 RC1

[Video](http://gr8conf.eu/Presentations/Building-Grails-apps-w-Gradle)

~~
### Gradle Multi Project Build

Gradle really shines at multi-project build. 

~~~~
## Groovy

Groovy is bigger then just Grails. There are many new features that have been added recently.

~~
### @DelegatesTo

This new annotation allows for better DSLs to be built. Using this annotation along with static compilation you can type check your DSLs. If you are using IDEA you even get autocomplete.

[@DelegatesTo Docs](http://groovy.codehaus.org/The+@DelegatesTo+annotation)
[Example Usage](https://github.com/ratpack/ratpack/blob/master/ratpack-groovy/src/main/java/org/ratpackframework/groovy/handling/ClosureHandlers.java)

~~
### Meta Annotations

* Allows rolling up annotations. 
* Set defaults for annotation parameters.

[Docs](http://groovy.codehaus.org/Meta-annotations)

~~
### ASTs

Using ASTs for compile time meta programming. An in depth workshop.

The Repo has tags for each exercise and it's solution.
[Repo](https://github.com/melix/ast-workshop)

~~
### Groovy 2.1 Talk

Guillaume Laforge talked about everything new in Groovy 2.1

[Slides](http://gr8conf.eu/Presentations/Lift-off-with-Groovy-2.1)

~~~~
## Grails

Many great talks and the area I gave my talks in.

~~
### Transactions

A proxy object for services adds the transactional functionality but that means you can't call new Server() and get transactions.

[Video](http://gr8conf.eu/Presentations/Grails-Transactions) 

~~
### My Plugin Talk 

Details on all the different ways to work with forked or unreleased plugins. 

Video to come on InfoQ later this year.

[Slides](http://bit.ly/gr8-plugin)

~~
### My Static Checking Talk

Detailed notes on how to set up static checking and why we need it.

Video to come on InfoQ later this year.

[Slides](http://bit.ly/gr8us-static)

~~
### Node Tools

How to use a ton of the front end focused tools that are built out in Node with your grails project.

[Slides](http://www.slideshare.net/zanthrash/node-tools-for-your-grails-toolbox-gr8conf-2014)

~~
### Hipster Talk

Want to use lots of new cool tools like vertx with grails?

[Example Project](https://github.com/sjurgemeyer/GR8ConfUS2013/tree/master/RobFletcher)

~~
### Extensible Testing Framework

This is a great intro to geb as well as a methodology to extend pages for a reusable system.

[Slides](http://www.slideshare.net/MikeEnsor/writing-an-extensible-web-testing-framework-ready-for-the-cloud-slide-share-21762477)

~~
### Good Form

A form tool for grails.

[Video](http://gr8conf.eu/Presentations/Good-Form---complex-web-forms-)
  
~~
### Searching for the Grail

Short answer use elasticsearch 

[Slides](http://gr8conf.eu/Presentations/Searching-for-the-Grail)

~~~~
## Ratpack

A new micro framework. Like sinatra. Allows a single file webapp using @Grab.

~~
### Example Single Page App

    @GrabResolver("https://oss.jfrog.org/artifactory/repo")
    @Grab("org.ratpack-framework:ratpack-groovy:0.9.0-SNAPSHOT")
    import static org.ratpackframework.groovy.RatpackScript.ratpack
    import org.ratpackframework.groovy.templating.TemplateRenderer

    ratpack {
        handlers {
            get {
                response.send "This is the app root (also try: /date and /some.txt)"
            }

            get("date") { 
             response.send "Hey date area"
           }
        }
    }
  
~~
### Testing Support Hackathon GR8EU

At the GR8EU Confernce I participated in a hackathon and helped add testing support to Ratpack.

[Example Test](https://github.com/robfletcher/midcentury-ipsum/blob/master/src/test/groovy/app/FunctionalSpec.groovy)

~~
### Ratpack Example App

[App](https://github.com/robfletcher/midcentury-ipsum)


