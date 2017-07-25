7/25/17 Karen Liu HTML/CSS Code Samples

## The Difference Engine

##### Each webpage of our client's app depended on various files from a Ruby on Rails app, so for the full sample, I've pasted code from the HTML, CSS, and Javascript in one place. When extracted and pasted together like this from the Rails app, it isn't fully usable, interactive, or representative of the original UI, but it does give an idea of what it looked like. I've compiled a preview of the HTML and CSS components blow. Please refer [here](https://github.com/KarenAF/HTML_CSS_Code_Sample/blob/master/full_samples/TDE/ListWithUs.html) to see the full sample for the 'list with us' page and [here](https://github.com/KarenAF/HTML_CSS_Code_Sample/blob/master/full_samples/TDE/homepage.html) for the full sample for the homepage, with the client name redacted.
About the development process at The Difference Engine: We worked in teams of about 5-7 developers, each working with a specific client to build their website or app. Most teams used a combination of the following technologies, but not limited to: Ruby on Rails, PostgreSQL (or another database), JavaScript on AngularJS, various API's, JSON, Bootstrap, Materialize, Email API's, Google Maps, Twilio, Action Cable, etc. We worked in two to four week Agile sprints and met with our clients once or twice a month. We used Slack for communication, GitHub for version control, and Heroku for deployment. 

**'List With Us' Page**
### CSS:
```
.list-content {
  position: relative;
  width: 75%;
  left: 10%;
  background: #F2F2F2;
  margin: 10px;
  box-shadow: 5px 5px 5px #888888;
  padding: 10px;
}

.arrow-steps {
  display: flex;
  margin-bottom: 20px;
}
```

### HTML:
```
<h1>List With Us</h1>

<div class="list-content">
  <h3>Intro</h3>
  <p>Donec egestas justo id pellentesque venenatis. 
  Etiam dapibus diam arcu, sit amet posuere ex venenatis in. 
  Phasellus dignissim nulla nec consectetur tempor. 
  Quisque venenatis, nulla at bibendum porttitor, 
  turpis justo sodales neque, 
  eget placerat justo purus congue massa. 
  Praesent lobortis tristique est ut euismod. 
  Nulla aliquam varius urna quis posuere. 
  Integer commodo ex nulla, a accumsan nibh dapibus mattis. 
  Aliquam et sodales ante.</p>
</div>


<div class="list-content">
  <h3><span id="list-title">THE HOME SALE PROCESS</span></h3>
  <div class="arrow-steps">
  <div class="step current" id='one'">
    <span>Step 1</span>
  </div>
  <div class="step" id='two'>
    <span>Step 2</span>
  </div>
  <div class="step" id='three'>
    <span>Step 3</span>
  </div>
  <div class="step" id='four'>
    <span>Step 4</span>
  </div>
  <div class="step" id='five'>
   <span>Step 5</span>
  </div>
  <div class="step" id='six'>
    <span>Step 6</span>
  </div>
  <div class="step" id='donation'>
    <span>Donation</span>
  </div>

```
![listwithus](https://github.com/KarenAF/HTML_CSS_Code_Sample/blob/master/img/ListWithUs.png)


**Homepage**
### HTML:
```
        <%= link_to image_tag('/images/mansion.svg', 
        :class => 'navbar-brand'), "/homepages" %>

        <button type="button" class="navbar-toggle collapsed" data-toggle="collapse" 
       
       data-target="#bs-example-navbar-collapse-1" aria-expanded="false">
          <span class="sr-only">Toggle navigation</span>
          <span class="icon-bar"></span>
          <span class="icon-bar"></span>
          <span class="icon-bar"></span>
        </button>
        <a class="navbar-brand" href="/homepages">Client Name</a>
      </div>

      <!-- Collect the nav links, forms, and other content for toggling -->
      <div class="collapse navbar-collapse" id="bs-example-navbar-collapse-1">
        <ul class="nav navbar-nav">
          <li class="active"><a href="/properties/">Find Your Home
          <span class="sr-only">(current)</span></a></li>
          <li><a href="/listwithus">List With Us</a></li>
          <li><a href="#">Company</a></li>
          <li><a href="/charities/">Charities</a></li>
          <li><a href="#">Contact</a></li>
          <li><a href="#">Client Investor</a></li>
        </ul>

```
![listwithus](https://github.com/KarenAF/HTML_CSS_Code_Sample/blob/master/img/homepage.png)







