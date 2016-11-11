# CDS
Chrome DevSummit Notes

## KeyNote
> The state of Chrome and the Web Platform today, from the leader of the Chrome team.

Darin Fisher's (VP of Chrome Engineering) keynote:

* Mission: Move the web platfrom forward.
* Over 2 billion active Chrome users across mobile and desktop.
* Not just Chrome, the Web has a reach!
* Links the Web's superpower, physical becons. [Polymon](https://polymon.polymer-project.org/)
* Every inteaction step costs 20% of your potential users! 
* The Web is Mobile: Constrains has lead to innovation. 
* Build for Mobile Web is a priority: Connectivity constraints 
* Almost 60% in developing market are on 2G! 
* 230M in US, 460M in India (100M new users every year!) 760M in China.
* 65% of Indian population aren't online yet, 20% in US are not yet online. 
* Web works well really well in emerging markets: Flipkart, Voot Viacom18.
* Progressive Web Apps: Radically improving web experince. Not able on technology, it's more about new way of building web experince. 
* Demo on [cnet-tech-today](http://cnet.com/tech-today) a progressive webapp.
* Alibaba usecase study: 76% higher conversion due to progressive webapp; Singles day is an event in China on November 11th is the biggest event on the internet, 3times more than cyber Monday, is on a progressive webapp.
* Fast - 53% of users abandunt the site which takes more than 3 seconds to load. 
* Refresher on service worker API. 
* The Monica Per Test gets a mention. 
* Apps should be interactive within 5seconds over 3G.
* Engaing - Add to Home screen; 4x more engagement due to this feature; prompting users sooner yields 48% more installs. 
* Install vs ATHS.
* Improving ATHS flow so the website will be in all apps location. 
* Ability to update the home screen icon or the name. 
* Push notification: 18 Billion push notifications sent everyday over 50,000 domains using it! 
* Seamless Sign-In: 85% redcution in sign in failure for AliExpress, Pinterest 10% increase in desktop logins. 
* WebPayments: Payment request API. 
* Productivity: Lighthouse, Real World condition testing, Security and Applications panel in Chrome. 
* Polymer gets a mention. 
* [Beta webcomponets](https://beta.webcomponents.org/) and AMP. 
* Predictability: The web should just work for developers. [browser-issue-tracker-search](https://browser-issue-tracker-search.appspot.com/)
* Looking ahead: Web assemebly, WebGL 2.0, WebVR, WebAR, WebBluetooth. 

## Building Progresive Web apps.
> Thao Tran, talks about it.

* Looking back from the previous year to this in the progress of progressive webapp.
* Toys lasts for a week! Was the Flipkart PWA a unicorn, not really! 
* Beyond Flipkart the overall momentum went up. 
* 17K across 35 countires for a PWA summit. 
* What is a PWA? Radically improving web user experiences; It's a joureny; 
* [building-indexable-progressive-web-apps](https://webmasters.googleblog.com/2016/11/building-indexable-progressive-web-apps.html)
* Housing.com Android App -> $3.75 and Mobile Web -> $0.07; 30% faster page load; 38% increase in conversion. 
* Early beta of [web elm](https://mobile-beta.westelm.com) PWA.
* Infobase Latin America: 65% of traffic is on mobile, < 1s page load time. 
* Lyft rolled out an mobile site just to test orders: they had 5x more rides from mobile web! So they are building a PWA which will be `<1MB` compared to 17MB andoird and 75MB ios.
* MakeMyTrip: Same day reservation from mobile web, PWA users book 3x more on their first visit! 
* The Weather company (An IBM Business): 18months ago they started: Moved to HTTPS, Web Push notification, 178 countries in 62 languages now!
* PWA: Acquistion; Engagement; Conversion; Retention.


## Sign-in on the web; crendtial management API
> Sabine and Eiji share best practices for sign-in, and explains how the Credential Management API makes frictionless sign-in possible.

* Removing friction
* Growth: 54℅ will abandon rather than register.
* autocomplete inputs.
* Avoiding login friction: 92℅ leave the site if they can't recall the password.
* Leverage the power of the browser to make sign-up easier with credential management API.
* Session management and 2 cookie handoff using serviceworkers.
* Launched in Chrome 51.
* Problems that this API solves:  Auto sign-in, Smart lock for passwords.
* Auto sign-in across devices.
* Supports multiple accounts.
* Virtually enables a permanent
* Remembers federated accounts.
* Steps: Interrupt the from submission; send an Ajax request; store the credential information; update the UI.
* Federated login cases: Auth; store the identity information; store the credentials.

## Faster payments.
> One of the hardest web user experience challenges is enabling users to make payments. Zach shows us how with the new Web Payment API.


* Save the world from annoying checkouts form.
* PaymentRequest API: Not a new payment method; Not a gateway or a processor;
* Fundamentally build for users, is a standard-based API making payments easier for users.
* Main goals: Easy checkout and secure payment on Web.
* Supported data types: Credit cards and Android pay; Shipping address, options, phone, email, payer name.
* All the data points are stored and returned from the browser.

## Debugging The Web.
> Learn the state of the art in debugging using Chrome DevTools - all you need to know to expand your toolbox.

* Debugging like a boss: Making it clear on why there was an issue right on the devtools. In Chrome55+ the screen orientation will not affect the content much. 
* ES6 + DevTools.
* Text editor like REPL in DevTools.
* Better autocompletion on Objects.
* Substrings completions are better.
* Snippets....
* Place multiple inline break points in async or any line of code.
* Auto picks up the workspace mapping on drap and drop. (*Source maps)
* CSS coverage. Unuse CSS.
* NodeJS main context debugging in the same devTools.
* Application tab > manifest, clear storage, servicework et.al.
* Audting PWA: Audit2.0 uses the power of Lighthouse. 

## Polymer, Web Components & You.
> Taylor Savage and Monica Dinculescu on the current state of Polymer, and how you can use Web Components to improve your development.

* Mobile device constraints. 
* Use the platform.
* Primay focus of Polymer are web-components. 
* Web Components V1. (Cross browser web component)
* Polymer 0.5 was an experiment, 1.0 was production-ready, 2.0 shall be web native.
* Who is using Polymer: Comcast, ING, BBVA, Netaporte, Coca-Cola, EA, Predix, Google and others. 
* Polymer App Toolbox: Set of web components, CLI, PRPL pattern; Example -> [shop](https://shop.polymer-project.org)
* JUMIA Travels use case: 75% of mobile connection is on 2G in Africa, >2x faster page load on 2G and 6x less data than native app.
* What's next on ploymer? Polymer2.0 - Web component V1 support; Better interoperability; Minimally breaking (backwards compatibility); Supports hybrid mode (i.e both on V1 and V2). 
* Polymer is light, it's just 12kb. 
* Polymer is about elements! element development is hard; Authors, maintainers and users of elements are the player here.
* 100+ elements in polymer; 3 orgs; 20+ apps; 500+ projects.
* Steps: Think of the features; Map the features to components; 



## Progressive Performance.
> Alex Russell on the important things to focus on in performance, and how to run great experiences on slow, inconsistent networks and low-power devices.

* [I realized I'd invented webpages](xkcd.com/1367)
* We are in the middle of a crisis. 
* RAIL: 100ms/8ms/50ms chunks/1000ms.
* 53% bounce with sites that take more than three seconds to load. 
* Collectivily we are failing;
* Why are our tools slow?
* Your laptop is a filthy liar. 
* Understand the depth of the deficit. 
* The truth is in the trace. 
* Avg selling price of smart phones are going down; The next million users are buying their first phone.
* Motion Mark: Desktop version is like 25x times faster. 
* Power = Heat.
* A desktop can emit 60W of enegry; Mobile devices can't do that!
* No termal paste, no fans, no heat sinks on a mobile device. 
* Dark silicon and the end of multicore scaling paper. 
* 10.0Wh is all the battery got and it has to deal with GPU, CPU, NFC, Screen, Wifi et.al
* big.LITTLE arch. 
* "touch boost"; SMP vs HMP vs EAS. 
* Benchmarketing is A Thing! (Can't trust them)
* Mobile CPUs aren't really what think they are. 
* MLC Flash is how we make storage cheaper. 
* Read Perf: MBP: ~2GB/s and N5X: ~400MB/s.
* Mobile networks hate you! 
* Will LTE save us? Networks are slowing down. 
* Network overhead of one HTTP request! 
* Load less code, load it at the right time and let the browser help us whenever we can. 
* Ignorance / Priviliage or both is the result of the frameworks today.
* Tools that doesn't use platfrom well, we endup in the Uncanny Valley. 
* Serviceworkers aren't just about offline experience it's also about reliable performance! 
* Mobile Hates You; Fight Back! 

