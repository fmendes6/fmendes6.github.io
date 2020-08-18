+++
title = "Xamarin First Impressions"
date = 2014-04-10
author = "fmendes6"
draft = false
+++

It has been 13 months since I started developing for Android and until now I have been using eclipse/IntelliJ as my IDEs, however, a new professional commitment made me to develop for Android using Xamarin and this blog post discusses my first impressions that i’ve experienced as an Android developer with Xamarin.

“With Xamarin, you write your apps entirely in C#, sharing the same code on iOS, Android and Mac” is Xamarin’s moto as a platform to develop iOS and Android with C# instead of Objective-C or Java respectively.

## But why developing with C# (xamarin) instead of developing with the language that Android was designed for?

Although one reason may be that the developers are not familiar with Java, the most important (in my opinion) is the possibility of developing with the benefits that C# has over Java (delegates,linq,async operations,etc.). After all, i can assure you that the code looks clearer and is easier to develop.

On the other hand, it enables us to develop the application core (business logic and data access) that is separated from the UI, and gives us the possibility to reuse that code within various client applications (Android, Windows, iOS).

## Well ok but...How does it work?

Xamarin lets us to develop everything with C# as long as we know how does the whole Android ecosystem works. It is necessary to understand the 4 basic components (Activity, Services, Broadcast Receivers and Content Providers) and how they work together. Even the types and methods are named same as in Java so that the only difference is the language in which one develops.

However, as someone who usually develops in Java, I realized quite quickly that a slight learning curve which was one of the noticeable differences. This was the use of custom attributes in activities in order to define their attributes (that is name, screen orientation, etc) instead of defining them in the manifest file. Also, as I noticed, there is a use of Properties instead of setter methods as in Java (ex: button.click += delegate {...} instead of button.setOnClickListener(...))

## Wow! That seems cool! So how do we start?

That is where the problems begin...

### Visual Studio:

I decided to start with Visual Studio since it is an IDE that I like a lot and that I had installed already because of my previous projects. The only necessary thing was to add a plugin (available for business accounts only).

After installing the plugin it is necessary to associate the business account with the Visual Studio int the menu options. The problem was that those options didn’t open because of a plugin error. After more than one hour (thanks to the deletion of one entry in the system registry), I managed to configure the account and deploy an Android application to my Nexus 4. But instantly Visual Studio warned me that LogCat would not be available for that application.

After this warning, I gave up with Visual Studio and decided to give Xamarin Studio a try.

### Xamarin Studio:

At first glance it seems to be a fast and simple to use IDE. Without any greater difference from the other IDEs, it doesn’t require a great learning curve, which is good!

The first weird crash that occurs is related to the save file operation. From this point on, the sporadic weird crashes started to occur more frequently although on simple and fast IDE reset solved the issue.

By the time I started to develop my own layouts, i realized that the IDE has no auto-complete feature in the XML files (or AXML as Xamarin “calls” it).

- SH\*T.

Being an avid user of the auto-complete feature, since it helps with productivity, I perceived the above as a problem.

After a short research on the Xamarin forums, I learnt that some users find it possible to turn this feature on but only if we open it with a right-click and choose “Source Code Editor” (instead of a typical double-click on the .axml file). This way we enable auto-complete only on the attributes (but not on their values).

However, opening it with “Source Code Editor” removes the “Design” tab. That makes it necessary to double-click the file (again) to access and view the result.

This means that double clicking the file enables us to access the design tab and the source tab without auto-complete. Opening with “Source Code Editor” provides us with auto-complete but without the design tab. This did not appear as productive to me...

Then my co-workers suggested me an interesting solution. We shall use Android Studio (or IntelliJ) to develop the layouts, (taking advantage of the awesome “preview” tab that enables us to edit a layout file and looking at the results in real time) and then copy the above to xamarin studio, since those XML files are defined with the same rules and definitions.

Of course, keeping both IDEs opened together with chrome and other apps at the same time, demands at least a system with 8GB of RAM so that the development is prompt and possible at all.

## Hum OK... Is there anything more that we should learn?

Well yes, there is. If you are thinking about using 3rd party Java libraries (.JAR) or Java projects, then you have several ways to do it:

- Converting them manually;
- Using code converters
- Using the Java Native Interface;
- Through a specific library that defines the mapping between Java and C# (Java Binding Library).

All these options are well described on Xamarin official website.

## Well...with so many problems is Xamarin still worth it?

This decision can only be made by you. Nevertheless, if you are planning to share code across multiple mobile OSs, then Xamarin seems to be a really good option for me, even with the mentioned limitations in mind, as long as we use it together with Android Studio/IntelliJ to design the layouts :P

That is all for today. In the following weeks, I am going to write another blog post. This time enriched by a greater experience with Xamarin. So shall we keep in touch? :)

## Update (22/06/2014)

With Visual Studio 2013 (12.0 update 2 at least) and the Xamarin plug-in everything seems to work well! No weird crashes, the logging works perfectly and additionally it has got an intellisense for C# code, which Xamarin Studio hasn’t got. I had been using Visual Studio 11 by the time I had written this post so maybe there was some problem with it.

From now on, I would recommend Visual Studio 12 and Android Studio.
