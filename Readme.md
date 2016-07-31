## Help Me

![helpme logo](img/Helpmeicon.png)

Tag-line:  …Crisis Support Family and Disaster….we link to service providers… Virtual assistance..or I need Emotional Help now.

### Description

Help Me is an Well Being On Demand Application that connects vulnerable people with crisis support and services for emotional wellbeing. It is a tool that equipping everyone in Australia with the support and skills to protect their emotional wellbeing health - an on demand emotional wellbeing tool that uses technology to anonymously and  securely connects real people to real professionally qualified listeners for chat. Anyone who wants to talk about whatever is on their mind can quickly reach out to a trained, compassionate listener through our network. We have hundreds of listeners who come from all walks of life and have diverse experiences.

In 2014-15 there were 4.0 million Australians (17.5%) who reported having a mental or behavioural condition.

Help Me is an on-demand application connecting vulnerable people to crisis support 24/7. People connect with listeners on 7 Cups of Tea for all kinds of reasons, from big existential thoughts to small, day-to-day things that we all experience. Unlike talking to family or friends, a 7 Cups of Tea listener doesn’t judge or try to solve problems and say what to do. Our listeners just listen. They understand. They give you the space you need to help you clear your head.

The virtual assistant algorithm is sympathetic to emotional feedback and tone of voice. Via interactive chat, the virtual assistant will recommend appropriate services whether it is an activity to try or connect to a professional who are available. Among the list of available professionals who are connected with Help Me, the most appropriated will be connected to the help seeker. Help me also provide directions to the nearest facility using augmented reality interface which is safer than looking down at a map on your phone while walking. Help Me also suggests wellness activities like meditation classes and the nearest parks for exercise and walks.

#### XMPP based real-time messaging

XMPP based library Strophejs has been used for real-time text transmitted instantly while it is being typed or created. The recipient can immediately read the sender's text as it is written, without waiting. This can be used in Help Me for two purposes - to interact with real professionals offering their free time for the community, and to interact with a bot which interfaces with an experimental empathetic subject matter specific virtual assistant which will try to determine and point out services which can come to the user's aid.

#### Subject matter specific virtual assistant (experimental)

There are two main elements to it that you set up within your app – intents and entities. An intent is what action an instruction should take (e.g. point to NGOs - like Lifeline support call centers - working with people in crisis in the immediate vicinity). An entity is a specific object or piece of information that our AI needs to know about to enact that intent (e.g. what kind of crisis support service?).

Wit.ai provides the service to convert verbal commands into text and can also be trained up in how to understand those commands. Wit.ai has the concept of “roles”, where it can learn to differentiate between entities in different contexts (e.g. numbers in different parts of an instruction can refer to different things – like age of the user). An experimental virtual assistant can be developed using services like Wit.ai and a XMPP based chat bot can be used to interface the user to the virtual assistant.

#### Augmented reality based geolocation, routing and navigation:

We have developed the proof-of-concept of a browser-based Augmented Reality app to locate services which are open at the time of use (of the app) around the user. This kind of app would be normally developed using native APIs of the mobile phone OS (Android/iOS/Windows Mobile) and is extremely complex. The key concept is to use the mobile device sensors, mainly accelerometer, magnetometer, GPS, camera to establish the current location, orientation and point-of-view (in terms of camera viewport) of the device. On top, of the camera feed on the phone screen, data is superimposed in transparent/semi-transparent layers. This is done by creating virtual markers based on geolocated dataset(s) and using algorithms to determine the approximate distance and direction of heading for the marker in relation to the user's (and phone camera's) point-of-view. Navigation features can be added by using the phone's motion sensors to determine direction of movement as well.

Since our proof-of-concept has been developed within the time constraints of Unleashed 2016, Adelaide and Govhack, it has been developed using HTML5 geolocation (GPS), the orientation API (accelerometer) and WebGL (GPU). This PoC currently requires a standards compliant mobile browser (e.g. Firefox on Android). iOS does not currently support WebGL or WebRTC and has not implemented the DeviceOrientation API correctly. Please see [this post to the W3C GeoLocation Working Group link](http://http://lists.w3.org/Archives/Public/public-geolocation/2014Jan/0000.html) for more detailed information. [Awe.js link] (https://github.com/buildar/awe.js/) has been used for building the app. A transparent overlay of Google Maps has been used to display roads and locate markers on top of the camera feed for simplicity.

Team name: Bob's gang

Team members: Matt Cejko, Martin Nobis, Muhammad Pavel, Mizanur Rahman, Asheshwor Shrestha, Oshim Somers

Demo url: https://github.com/Unleashed2016/helpme

Video url:

Hackerspace url: https://2016.hackerspace.govhack.org/content/help-me


### Local Event Location:

Adelaide

### Datasets Used:

* SA community services directory: https://data.sa.gov.au/data/dataset/south-australian-community-services-directory This data provides the list of available services for those seeking help through our app.

* ACNC registered charities: https://data.gov.au/dataset/acnc-register This data provides list of services available so we can refer those seeking help through our app.

* hospital specialist services: https://data.sa.gov.au/data/dataset/public-hospital-specialist-services/resource/fedc4ee4-de59-4147-b45f-42f145a446a3 This database provides is used to provide information on availability of specialists in public hospitals across South Australia which is used for referral through our app.

* Hospital locations in SA (SA Public and Private Hospitals Locations): https://data.sa.gov.au/data/dataset/sa-health-hospitals-locations Location of hospitals will be used to get directions to app users using maps and augmented reality

* GP locations data https://data.sa.gov.au/data/dataset/gp-plus-locations This database provides location of public and private hospitals in South Australia. This is used for referral through our app based on need and condition of the user.

* National Health Survey: First Results, 2014-15 http://www.abs.gov.au/ausstats/abs@.nsf/Lookup/by%20Subject/4364.0.55.001~2014-15~Main%20Features~Mental%20and%20behavioural%20conditions~32 The trends on prevalence of mental and behavioral conditions data was used to define the problem for the use cases.

* South Australian Monitoring and Surveillance System: Target, Trends at a glance & Indicator reports https://data.sa.gov.au/data/dataset/south-australian-monitoring-and-surveillance-system-target-trends-at-a-glance-indicator-reports The trends on prevalence of mental and behavioral conditions data and targets was used to define the problem for the use cases.

### APIs Used:

* Awe.js: Used to simplify using HTML5 geolocation, orientation and WebGL

* Three.js: Used as a cool WebGL library

* Google Maps JS API: Used to superimpose a layer of Roads and Streets with names on top of the camera feed.

* Google Maps Directions API: Used for routing and navigation from user's current location to destination

* Strophejs: JS API library for XMPP used for real-time chat service.

* Wit.ai (not used in the PoC): Wit.ai is a service which provides a combination of both voice recognition and machine learning. It provides the service to convert verbal commands into text and can also be trained up in how to understand those commands. Wit.ai has two main elements to it that you set up within your app – intents and entities.

* Backendless: On-demand Mobile Backend as a Service (mBaaS) platform.
