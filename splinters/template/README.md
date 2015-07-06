# CS19 Splinter Session Webpage Template

The Cambridge Workship on Cool Stars, Stellar Systems, and the Sun ("Cool Stars")
has a strong tradition of supporting independently organized parallel sessions
throughout the course of the workshop ("splinter sessions"). Cool Stars 19 in
Uppsala will not be an exception. To provide the best possible experience for
attendees of the Workshop and individual splinter sessions, we require that
splinter sessions compose a dedicated webpage with all pertinent information
about the session (date, motivation, speakers, schedule, etc).

Making a webpage from scratch can take a lot of time, as we can attest. To help
relieve effort on our part and the part of individual splinter organizers, we use
the Foundation 5 front end and provide this template. An added benefit is that
this allows us to homogenize the look and feel of events surrounding
Cool Stars 19. Below is some basic information on [Foundation 5](http://foundation.zurb.com/),
information about where to host your splinter webpage, and instructions on what
to change in the template, with highlights of a few particular features.  

### About Foundation 5

Foundation is a widely-used framework to build responsive and mobile-friendly
websites (used among others by Mozilla, the Washington Post, National Geographic).
We use Foundation 5 to serve the users and CS19 attendees a fast website, built
around modern standards, and that scales smoothly from large displays workstations
to smartphones. Foundation 5 provides a set of building blocks or components that are ready to use.
We use some of them in this template, which will be described below. More information
on the building blocks can be found on [Foundation 5 website](http://foundation.zurb.com/docs/)

#### Accordion

#### Interchange
Interchange is a feature that will load different type of content for different
sizes of screen. We use interchange in this template to display a simple text list
of invited speakers for small screens, and a fancy circular photo with affiliations
for medium- and large- sized devices.
![Interchange for small screens](www.astro.uu.se/~alavail/misc/interchange_small.png)
![Interchange for medium screens](www.astro.uu.se/~alavail/misc/interchange_medium.png)
A default text is specified in case
javascript is not allowed to run. Below is the code snippet

```html
<div class="row">
  <div class="small-12 columns">
    <h3>
      Invited speakers
    </h3>
    <div data-interchange="[small.html, (default)], [medium.html, (medium)]">
      <ul>
        <li>Greg Feiden (Unseen University)</li>
        <li>Alexis Lavail (Ministry of Love)</li>
      </ul>
    </div>
  </div>
</div>
```
For small screens, the content from "small.html" is loaded, for medium screens and large
screens, "medium.html" is loaded. In case scripts are not allowed to run, the html
within
```html
<div data-interchange="[small.html, (default)], [medium.html, (medium)]"></div>
```
 is displayed. Feel free to change the type of information you want to display.
 If you do not want to use interchange, and display the same content for any device,
 simply remove the outer
 ```html
 <div data-interchange="[small.html, (default)], [medium.html, (medium)]"></div>
 ```
element. Please keep in mind that a large number of people will access this webpage
with mobiles devices and tablets. Therefore, you should avoid loading heavy, and/or
large material on small screens.

### Where to Host

Where to host your splinter webpage is up to you, but there are really only
two options. First, you can host it on your institutes web server. Check with
your local IT department if you prefer this option. Second, we are happy to
host your splinter session webpage on our server along with the core of the
Cool Stars 19 webpage.

We recommend the latter option for purposes of longevity. The Cool Stars 19
web server will remain accessible for an indefinite period of time after the
conference. Therefore, splinter session pages that we host and information will
be archived and preserved for future reference.

### Usage

### Authors

[Alexis Lavail](https://github.com/astro-alexis)

[Gregory Feiden](https://github.com/gfeiden)

### Contact

[Cool Stars 19 LOC](mailto:cs19@physics.uu.se)
