Note: A lot of volunteer effort by individuals supporting the UWP Platform is represented in this list. When you can, please consider giving feedback to the authors, testing their code and filing issue reports/feature requests and hit the Star button for their project. If your favorite project is missing from this list, please let me know.


#  :ballot_box_with_check: The-UWP-Tools-List

UWP - Universal Windows Platform for Windows 10 Desktop, Windows 10 Tablets, Windows 10 Mobile Phones, Windows 10 Pixelsense, Windows 10 IOT, Windows Server, Windows 10 HoloLens, and Windows 10 Xbox.

Some UWP libraries are PCL based and should also work with Android and Apple IOS via Xamarin. PCL targeted at .NET 3 also work with Unity 3D as another way of targeting Android and IOS. This List is currently focused on Windows 10 devices but I'll try to call out other targets. The introduction of .NET Core should also help in this area.

On a Windows 10 Desktop or Tablet, a UWP App is typically deployed to a safe sandboxed environment via the Windows Store but the App can also be easily sideloaded to access legacy Windows 10 Desktop features and services with the [BCTemplates](https://github.com/lancecontreras/BCTemplates)  project being an example of one approach. This process has become very convenient with the Anniversary Update and is a simple setting in "Update & security" which makes a Windows 10 Tablet and Windows 10 Mobile device a very convenient deployment device for all kinds of touch based applications out in the "Real World"

This is extensive list (in progress) of potentially useful UWP Tools, Libraries, Samples etc to help make your UWP development more awesome. The list is non-curated (but with opininated comments when available). The ultimate objective is to provide a broad starting point for UWP development to perhaps help to offset the currently chaotic and sporadic information that is generally available.

All contributions are welcome. Try to include a Title, Link, Description but any comment is welcome. Adding an GitHub Issue is another low effort way to add something here. I'll even try to insert any editorial type comments you might want to share in order to make this document a bit more interesting to read over and above a rather dry list of projects.


# Microsoft


Note that current Microsoft Emulators are based on Hyper-V which is a low overhead VM technology. To painlessly fire up emulators, you need both a modern CPU that supports SLAT instructions and the "Pro" version of Windows 10.

### Microsoft Downloads and tools for Windows 10

https://developer.microsoft.com/en-us/windows/downloads

[Windows App Certification Kit](https://developer.microsoft.com/en-us/windows/develop/app-certification-kit) This is an often overlooked gem. If you have a .NET libary etc and want to know how much of you code depends on non UWP API, this tool can help.

[Windows 10 SDK] (https://developer.microsoft.com/en-us/windows/downloads/windows-10-sdk) This is required, but included with VS 2015. 

[Mobile Emulator](https://msdn.microsoft.com/windows/uwp/debug-test-perf/test-with-the-emulator)

[HoloLens](https://devoloper.microsoft.com/en-us/windows/holographic/development_overview) Get the tools you need to build apps for Windows, including holographic apps. There is no separate SDK for HoloLens; holographic app development uses Visual Studio 2015 Update 3 with the Windows 10 SDK (version 1511 or later). Don't have a HoloLens? You can install the [HoloLens emulator]() https://developer.microsoft.com/en-us/windows/holographic/using_the_hololens_emulator to build holographic apps without a HoloLens. We also recommend installing the Unity game engine as an easy way to get started creating holographic apps.

[Multilingual app toolkit](https://developer.microsoft.com/en-us/windows/develop/multilingual-app-toolkit)

[Badges](https://developer.microsoft.com/en-us/store/badges) create the HTML and get the artwork needed to promote your apps and content

[Microsoft Store Services SDK](https://visualstudiogallery.msdn.microsoft.com/229b7858-2c6a-4073-886e-cbb79e851211) Create A/B tests that you can run and manage in Dev Center. Launch Feedback Hub so customers can submit feedback and upvotes that you can review in Dev Center. Use the advertising APIs to display banner ads and video interstitial ads.

[OneDrive API 2.0](https://dev.onedrive.com/)

[Azure-adding a cloud backend to your mobile app](https://azure.microsoft.com/en-us/documentation/services/app-service/mobile/)

[Where is the DirectX SDK?](https://msdn.microsoft.com/library/windows/desktop/ee663275.aspx) DirectX is now a fundamental part of Windows.Starting with Windows 8, the DirectX SDK is included as part of the Windows SDK. We originally created the DirectX SDK as a high-performance platform for game development on top of Windows. As DirectX technologies matured, they became relevant to a broader range of applications. Today, the availability of Direct3D hardware in computers drives even traditional desktop applications to use graphics hardware acceleration. In parallel, DirectX technologies are more integrated with Windows. 

[Microsoft Lumia SDKs](https://developer.microsoft.com/en-us/windows/featured/lumia) SensorCore SDK 1.2 Preview & Imaging SDK 3.0

[VM - Get a Windows 10 development environment](https://developer.microsoft.com/en-us/windows/downloads/virtual-machines) Run this VM on your current Mac or PC for an evaluation of the Universal Windows Platform tools and technologies

[Windows 10 IoT Core](https://developer.microsoft.com/en-us/windows/iot/Downloads.htm)


### Code Samples

https://developer.microsoft.com/en-us/windows/samples

[Microsoft UWP Official Samples](https://github.com/Microsoft/Windows-universal-samples) This is is the main repo of Microsoft UWP samples. A multitude of tiny code bits showing every part of UWP.

[Windows.UI.Composition](https://github.com/Microsoft/WindowsUIDevLabs) With the deceptive name of "Windows UI dev labs" this repo contains code samples, demos, experiments, prototypes, and preview explorations that show how to use Windows.UI.Xaml and Windows.UI.Composition to make beautiful UWP applications. 

[Win2D](https://github.com/Microsoft/Win2D/archive/master.zip) Win2D is an easy-to-use Windows Runtime API for immediate mode 2D graphics rendering with GPU acceleration. It is available to C# and C++ developers, and utilizes the power of Direct2D, integrating seamlessly with XAML and CoreWindow.

[DirectX 12 graphics samples](https://github.com/Microsoft/DirectX-Graphics-Samples) DirectX 12 Graphics samples that demonstrate how to build graphics intensive applications on Windows.

[Windows task snippets](https://github.com/Microsoft/Windows-task-snippets) Snippets of ready-to-use code that accomplish small, but useful, tasks of interest to UWP app developers. These snippets show simple solutions to common problems, and simple recipes to help you implement new app features.

[Photo Sharing App](https://github.com/Microsoft/Appsample-Photosharing) UWP app sample that demonstrates real-world social media experiences around photo sharing.

PhotoSharingApp is a Universal Windows Platform (UWP) app sample that demonstrates real-world social media experiences around photo sharing.

With this app, users can earn virtual gold by uploading and sharing photos with people from all around the world. They can upload photos of their cats, shoes, houses, or last vacations, and see how they compete against other users. Are their photos a great gold source? Are they among the most generous contributors? They can find out on the app's leaderboard.

The goal of this app is to provide a complete, end-to-end example of a real-world app that uses a variety of UWP features, and exhibits design and development best practices. This makes it a great source of code you can copy into your own apps. It also provides an example of what a real-world app architecture might look like. The decoupled architecture makes it easy to reuse code or to make changes and build your own photo sharing app, which you can then publish in the Windows Store.

![](https://github.com/Microsoft/Appsample-Photosharing/raw/master/Images/Category-Overview-Desktop-Mobile.jpg)

-    Browse photo categories and navigate into photo collections and photo details.
-    Take and upload photos directly in the app or upload an existing photo.
-    Give gold and add comments to photos uploaded by other users.
-    Receive push notifications when users are given gold for uploaded photos.
-    Explore a leaderboard of users with the most gold, users that have given the most gold to other photos, and the photos that have received the most gold.
-    Sign in with a Microsoft, Facebook, Google, or Twitter account.
-    Report content as abusive, inappropriate, or spam.
-    Buy virtual gold using in-app purchase.

- Adaptive UI using the SplitView control (see video on Channel 9) and adaptive triggers:
- In-app purchase (see the Windows.ApplicationModel.Store namespace):
- Separation between user interface, business logic and data models (MVVM):
- Extensibility and flexibility using the Unity dependency container:
- How to connect your app to an Azure App Service
- Real-world service implementation for storing uploaded photos using Azure DocumentDB
- Sign-in with Azure Mobile Apps:
- Usage analysis with Visual Studio Application Insights
- Push Notifications (see Integration with App Service Mobile Apps in Azure Notification Hubs:

[Rss Reader](https://github.com/Microsoft/Windows-appsample-rssreader) A UWP app sample for retrieving RSS feeds and viewing articles, demonstrating adaptive layout and hierarchical navigation patterns.

![](https://github.com/Microsoft/Windows-appsample-rssreader/blob/master/RssReader.png)

- The navigation menu (hamburger menu) pattern and screen-width adaptivity using the SplitView control and the AdaptiveTrigger class.
- The Syndication APIs (Windows.Web.Syndication) to retrieve RSS feed data.
- The DataContractSerializer class to save and restore app data from local storage.
- C# and XAML using the MVVM design pattern.

March 2016 update:

- A complete redesign of the UI to show effective use of color, type, images, and animated effects.
- Major improvements to layout, navigation, and window-size adaptivity to support small and large screens.
- Use of the WebView control to show articles within the app.
- The ability to rename feeds and to rearrange feeds and favorites.

We implemented the navigation and layout patterns in this sample using code from the XAML navigation menu and XAML master/detail samples in the Windows-universal-samples repo. These samples represent the current minimum recommendations for these patterns, and the RssReader sample will continue to reflect this guidance in future updates. 

[Family notes](https://github.com/Microsoft/Windows-appsample-familynotes)

FamilyNotes is a Universal Windows Platform (UWP) app sample that explores different input modalities and scenarios of user awareness. The FamilyNotes sample is essentially a bulletin board app that allows family members to leave notes for each other on a common PC/tablet just like they would a bulletin board. Using text, speech, ink, or pictures, a user can create a note and tag it for another user. Later when that other user approaches the PC/Tablet, the app uses imaging APIs and the Microsoft Cognitive Services (Face API) to detect their presence and display the notes that have been left for them, effectively filtering based on facial recognition. While the app is open, users can naturally interact with it using speech (“Add note for Bob”). If the app isn’t open, a user can easily launch it and interact with it using Cortana.

![](https://github.com/Microsoft/Windows-appsample-familynotes/raw/master/Screenshots/Using_Ink_Voice_and_Face_Recognition_in_a_UWP_App_Video.PNG)

![](https://github.com/Microsoft/Windows-appsample-familynotes/raw/master/Screenshots/FamilyNotes.PNG)

-    Speech recognition and speech synthesis by using the SpeechRecognizer and SpeechSynthesizer classes.
-    User detection using the MediaCapture and FaceDetectionEffect classes.
-    User facial recognition using the Microsoft Face API.
-    Activation through Cortana voice commands, defined in VoiceCommands.xml (a VCD file), using VoiceCommands and Activation classes.
-    Pen input using the InkCanvas API
-    JSON serialization using the DataContractJsonSerializer class.
-    Setting the app wallpaper using the Bing image of the day task snippet.

[Hue light controller](https://github.com/Microsoft/Windows-appsample-huelightcontroller)

HueLightController is a Universal Windows Platform (UWP) app sample that explores integrating Windows features with intelligent home automation. Specifically, it shows how you can use Cortana and Bluetooth Low Energy (Bluetooth LE) to create an interactive experience with the Phillips Hue Lights (a Wi-Fi enabled lighting system). 

With Cortana integration, users are able to naturally interact with the lights through speech. They can turn the lights off, change their color, or even engage with Cortana in a back-and-forth conversation to adjust a specific light or change all the lights at once.

![](https://github.com/Microsoft/Windows-appsample-huelightcontroller/raw/master/Screenshots/Connecting.png)

Additionally, through Bluetooth LE, the app supports a proximity scenario where the lights are automatically turned on/off depending on a user's device relative to a Bluetooth LE beacon. 

-    Using the HttpClient methods and Newtonsoft.json to interact with the Hue lights' RESTful interface.
-    Extending Cortana to provide an intuitive voice interface for manipulating the lights.
-    Using BLE APIs in the background to watch for a BLE beacon indicating proximity to the lights.
-    Showing an extended splash screen for more time while the app connects to the Hue hub and searches for lights.


[Traffic app](https://github.com/Microsoft/Windows-appsample-trafficapp) and the [MVVM Version](https://github.com/Microsoft/Windows-appsample-trafficapp/tree/MVVM)

Traffic App is a sample Universal Windows Platform (UWP) app for commuters to track drive times to various locations. The user adds frequently-visited destinations using app-bar buttons or by tapping and holding on the map. Traffic App then provides a quick view into how long it will take to drive to each place from the user’s current location, following the fastest route. The user can also flag a particular destination and a background task will periodically monitor traffic to that location, alerting the user when traffic is adding ten minutes or more to the travel time. 

![](https://github.com/Microsoft/Windows-appsample-trafficapp/raw/MVVM/Images/TrafficApp.png)

-    MapControl and MapItemsControl (Windows.UI.Xaml.Controls.Maps)
-    Geolocator (Windows.Devices.Geolocation)
-    MapLocationFinder and MapRouteFinder (Windows.Services.Maps)
-    Background tasks (Windows.ApplicationModel.Background)
-    Toast notifications (Windows.UI.Notifications)
-    Local storage and serialization (Windows.Storage)

[Network helper](https://github.com/Microsoft/Windows-appsample-networkhelper) NetworkHelper library and Quiz Game

NetworkHelper is a sample library that demonstrates the use UWP networking APIs to enable network discovery and communication in your games or apps. Specifically, the library provides the ability for:

-    Wi-Fi network discovery and management peer clients over a local Wi-Fi network.
-    Direct communication between discovered devices on the same Wi-Fi network with developer configurable messages.

![](https://github.com/Microsoft/Windows-appsample-networkhelper/raw/master/Screenshots/QuizGame_JoinGame_scaled.png)
![](https://github.com/Microsoft/Windows-appsample-networkhelper/raw/master/Screenshots/QuizGame_GameInProgress_scaled.png)

QuizGame is a Universal Windows Platform (UWP) app sample that uses the NetworkHelper library to enable a pub-style trivia game. When running the sample, you are presented with an option to create a new game as a quiz master on your local network or join an existing game and answer questions from the quiz master. Questions appear on the quiz master's screen while players answer the questions on their own devices. A quiz master can advance the game to additional questions and display the scores at the end. Below are some features that QuizGame uses.

-    Simple MVVM (Model, View, ViewModel) coding pattern
-    Simple navigation using code-behind files.
-    NetworkHelper to enable discovery and broadcasting of available games on the local network.
-    NetworkHelper to enable communication between the game and players.


[Marble Maze](https://github.com/microsoft/Windows-appsample-marble-maze)

Marble Maze is a sample Universal Windows Platform (UWP) and DirectX app that demonstrates how to build a basic 3D game using DirectX. This game is a simple labyrinth game where the player is challenged to roll a marble through a maze of pitfalls using tilt controls.

This sample is written in C++ and requires some experience with graphics programming and DirectX. Complete content that examines this code can be found at Developing Marble Maze, a game in C++ and DirectX.

![](https://i-msdn.sec.s-msft.com/en-us/windows/uwp/gaming/images/marblemaze.png)


-    Incorporating the Windows Runtime into your DirectX game
-    Using DirectX to render 3D graphics for display in a game
-    Implementing simple vertex and pixel shaders with HLSL
-    Developing simple physics and collision behaviors in a DirectX game
-    Handling input from accelerometer, touch, and mouse, and game controller with the Windows Runtime and XInput
-    Playing and mixing sound effects and background music with XAudio2

See Also: [Developing Marble Maze, a UWP game in C++ and DirectX](https://msdn.microsoft.com/windows/uwp/gaming/developing-marble-maze-a-windows-store-game-in-cpp-and-directx)

[Office 365 code samples](http://dev.office.com/code-samples) integrating Office 365 data and services into your app

[UWP Community Toolkit](https://aka.ms/uwptoolkit) See description in Controls section


# Information
[awesome-uwp](https://github.com/tomzorz/awesome-uwp) Awesome UWP resources - inspired by Awesome .NET. - It appears to be a normal "awesome-style" "curated" list whereas [The-UWP-Tools-List](https://github.com/10UWP/The-UWP-Tools-List) is an attempt to include all possibly useful UWP tools and code. Over time, I hope to have just about everything I can find on GitHub and anywhere else so examine all code carefully before using (but the great glory of open source is that the code speaks for itself) and make sure it has a license you are happy with.  

# Tools

Note to add some actual Tools that might be handy for UWP development.

[IconCreatorForUWP](https://github.com/JuniperPhoton/IconCreatorForUWP) IconCreator helps you (developers) create icons of you UWP apps. Just simply import your .png icon file and click the start button. 

[AppxInstaller](https://github.com/aL3891/AppxInstaller) This repostitory was created in respose to some misconceptions and incorrect information about the universal windows platform (UWP) apps, specifically with regards to their dependency on the windows store and suppsed inability to be distributed outside it. This folder contains a powershell script, Generate-AppxMsi.ps1, that packages an appx file into an msi. It will also embed an installation script that will enable sideloading in the registry, trust the application cert if it is not already trusted and deploy the application. Currently this script is a proof of concept with hardcoded values, but later on it will be able to wrap any appx or appx bundle like this and read all the relevant information from the package directly. Appx installer is a file handler for appx files. Using it, when a appx file is double clicked, a window is shown with information about the app. The user can then click install to install the app.




# Database

[EntityFramework](https://github.com/aspnet/EntityFramework) Microsoft's recommended data access technology for new applications in .NET. The ONLY UWP option is SQLite and [it is a mess](http://ef.readthedocs.org/en/latest/providers/sqlite/limitations.html). [Getting Started on Universal Windows Platform](http://ef.readthedocs.org/en/latest/platforms/uwp/getting-started.html) (Opinionated Note: "Microsoft's recommended data access technology" has somehow ended up in the damaged situation of SQLite being the ONLY supported target for Microsoft's main thing, the Universal Windows Platform. The insanely stupid SQLite FK mess means that Entity Framework's Magic Unicorn (Migrations) becomes a useless broken technology on the One Microsoft platform that should count as the highest priority effort. UWP without an easy robust Microsoft supported data platform is a Microsoft blind spot that has been a drag on the success of the Win RT platform from the beginning. "You can workaround some of these limitations by manually writing code in your migrations to perform a table rebuild. A table rebuild involves renaming the existing table, creating a new table, copying data to the new table, and dropping the old table. You will need to use the Sql(string) method to perform some of these steps." (https://github.com/aspnet/EntityFramework/issues/329) There is an explanation in this issue: [ESENT database provider](https://github.com/aspnet/EntityFramework/issues/4423) which probably translates to "please hold" for another few months)  

### SQLite

[SQLite](http://www.sqlite.org/) SQLite is a software library that implements a self-contained, serverless, zero-configuration, transactional SQL database engine. SQLite is the most widely deployed database engine in the world. The source code for SQLite is in the public domain. Microsoft uses SQLite as a core component of Windows 10, and in individual numerous products. [System.Data.SQLite](https://system.data.sqlite.org/index.html/doc/trunk/www/index.wiki) System.Data.SQLite is an ADO.NET provider for SQLite.  Development and maintenance work is now mostly performed by the SQLite Development Team. The SQLite team is committed to supporting System.Data.SQLite long-term. [git mirror of SQLite](https://github.com/mackyle/sqlite) - [DB Browser for SQLite](https://github.com/sqlitebrowser/sqlitebrowser) Official home of the DB Browser for SQLite (DB4S) project. Previously known as "SQLite Database Browser" and "Database Browser for SQLite". Website at: http://sqlitebrowser.org

[Microsoft.Data.Sqlite](https://github.com/aspnet/Microsoft.Data.Sqlite) SQLite implementations of the System.Data.Common interfaces

[sqlite-net](https://github.com/praeclarum/sqlite-net) sqlite-net is an open source, minimal library to allow .NET and Mono applications to store data in SQLite 3 databases. It is written in C# and is meant to be simply compiled in with your projects. It was first designed to work with MonoTouch on the iPhone, but has grown up to work on all the platforms (Mono for Android, .NET, Silverlight, WP7, WinRT, Azure, etc.). Very simple methods for executing CRUD operations and queries safely (using parameters) and for retrieving the results of those query in a strongly typed fashion. Works with your data model without forcing you to change your classes. (Contains a small reflection-driven ORM layer.)

[SQLitePCL.raw](https://github.com/ericsink/SQLitePCL.raw) SQLitePCL.raw is a Portable Class Library (PCL) for low-level (raw) access to SQLite. This library is designed to be the common portable layer upon which friendlier wrappers can be built. Right now, every C# SQLite library writes their own P/Invoke and COM and marshaling and stuff. Build on this library instead and focus more on the upper layer and its goal of providing a pleasant, easy-to-use API for app developers. When people ask me to recommend a friendlier SQLite wrapper, sqlite-net is the one that I usually recommend. SQLitePCL.pretty is another friendly SQLite API wrapper. 

[SQLitePCL.pretty](https://github.com/bordoley/SQLitePCL.pretty) This library wraps the C like SQLiteAPI provided by SQLitePCL.raw with a friendly C# object oriented API. It adds an Async API. SQLitePCL.pretty has a very simple table mapping ORM, available in the SQLitePCL.pretty.Orm package on nuget. It supports inserting both new and existing objects, and finding and deleting objects by primary key, from SQLite database tables. Notably, the ORM is designed to make working with immutable data types much easier by supporting the builder pattern for deserializing database objects. Ineresting features include the ability to iterate through query result sets using LINQ, support for binary streaming of data in and out of SQLite using .NET streams, and a powerful async API built on the RX framework."

### ESENT

[ESENT](https://msdn.microsoft.com/EN-US/library/gg269181%28v=exchg.10%29.aspx) Extensible Storage Engine is built into and is available for use on every Windows computer and has been an approved DLL for Windows Store since Windows 8.0. Updates to the database are implemented with a transaction in order to ensure secure operations. ESE enables simultaneous access to multiple databases, including transaction-log file databases that can be used for system recovery. ESE is scalable to large or small applications. [ESENT Managed Interop](https://managedesent.codeplex.com/) it is not clear if the .NET wrapper is UWP compatible."It is clear. ESENT Managed Interop is compatible with UWP. Not all nuget package are, but core Interop package on nuget is compatible with UWP, I tested it myself and it work." Thanks to [Opiumtm](https://github.com/Opiumtm) for testing that.

### DBreeze

[DBreeze](https://github.com/hhblaze/DBreeze) - This has a native UWP DLL and is an *embeddable Database solution for UWP Apps* - http://dbreeze.codeplex.com/ - Professional, open-source, NoSql (embedded Key / Value storage), transactional, ACID-compliant, multi-threaded, object database management system for
.NET 3.5> / XAMARIN MONO / .NET Core / UWP (Universal Windows Platform). Written in C# .

### BrightStar

[BrightstarDB](https://github.com/BrightstarDB/BrightstarDB) BrightstarDB is a native .NET RDF triple store. It uses dotNetRDF to provide support for a wide range of RDF syntaxes as well as SPARQL query support. In addition to providing a raw RDF-based API, BrightstarDB also provides support for binding RDF resources to .NET dynamic objects; and a contract-first entity framework that enables the use of LINQ rather than SPARQL for query purposes.

### Marcello

[MarcelloDB](https://github.com/markmeeus/MarcelloDB) .net/mono/xamarin/winrt in-process object database. MarcelloDB is a mobile NoSql database. It is very light-weight with minimal memory footprint. MarcelloDB saves plain C# objects, including child objects, lists and collections. Not having to map your objects to the relational model can save you hundreds of lines of code. MarcelloDB is a pure C# implementation, so there is no need to package other binaries.






### LiteDB

[LiteDB](https://github.com/mbdavid/LiteDB) - http://www.litedb.org/-LiteDB - A .NET NoSQL Document Store in a single data file. LiteDB is now functional for UWP via PCL.

### Couchbase

[Couchbase](https://github.com/couchbase/couchbase-lite-net) - http://www.couchbase.com/ - http://developer.couchbase.com/mobile/ - The NoSQL database solution for mobile — everything you need to build always-available apps that work online & offline. Couchbase Lite is
a fully functional, on-device, lightweight, native, embedded NoSQL database. With Couchbase Lite, you have the full power of a Couchbase database locally on the device. You can create, update, delete, query, sync and much, much more.

#### Note:
Based on this GitHub issue: https://github.com/couchbase/couchbase-lite-net/issues/535 - Couchbase Lite for .NET will be available soon for UWP. "my goal is to still have it in 2016. After the 1.3 release we are going to assess platform support going forward (including the possibility of dropping some, which would free up time for UWP)."









#Data Other

[YAWL.Serialization](https://github.com/YAWL/YAWL.Serialization) Serialization helper library for Windows applications

[ObservableSettings](https://github.com/joseangelmt/ObservableSettings) Create a Settings class for UWP (Universal Windows Platform) that is observable, strongly typed and with default values.

[DynamicDataTemplate](https://github.com/kompiuter/DynamicDataTemplate) An example of how to dynamically select a data template based on the data type of an item, including examples in WPF & UWP.

[DevKit Xamarin Storage](https://github.com/rcervantes-dev/DevKit.Xamarin.Storage) DevKit Xamarin Storage is a library to save data serialized in local files, supported platforms: iOS, Android and UWP.

[DiscToolsUWP](https://github.com/DevTheo/DiscToolsUWP) no description, has DiscToolsLibUWP

[PCLStorage](https://github.com/dsplaisted/PCLStorage) PCL Storage provides a consistent, portable set of local file IO APIs for .NET, Windows Phone, Windows Store, Xamarin.iOS, Xamarin.Android, and Silverlight. This makes it easier to create cross-platform .NET libraries and apps.

# Templates

[Template10](https://github.com/Windows-XAML/Template10) Making Windows 10 apps awesome

[2016MVA-Template10](https://github.com/Windows-XAML/2016MVA-Template10)

[HamburgerTemplateUWP](https://github.com/StefanJanssen95/HamburgerTemplateUWP) A Hamburger Template for Visual Studio 2015 UWP

[UWP-Attached-ViewModel-Behavior-Template](https://github.com/espenrl/UWP-Attached-ViewModel-Behavior-Template)

[BCTemplates](https://github.com/lancecontreras/BCTemplates) Brokered Component Templates for UWP. These template includes client, server and proxy project and a starterkit which is a solution that contains those three projects. These are the basic projects needed to create a brokered component application. 


[WAT-UWP](https://github.com/sozercan/WAT-UWP) Web App Template (WAT) is Visual Studio 2015 project that lets developers create Universal Windows Platform (UWP) apps based on existing web content. Used in the right way, WAT can facilitate the creation of compelling extensions to your web content for Windows users.

[UWPNavBasics](https://github.com/kbfoot/UWPNavBasics) A replication of the Windows navigation sample for UWP with some tweaks to create a basic template

[UWPAppSkeleton](https://github.com/dkackman/UWPAppSkeleton) Project Template for an MMVM Light universal app that will create the skeleton of an app that looks and feels a lot like the built in Microsoft Windows 10 app (Weather, NFL etc). It's got all the basic stuff plumbed out like navigation and a navigation control, a settings page, Theme switch etc.

[UWPProjectTemplates](https://github.com/mspviraj/UWPProjectTemplates) Visual Studio 2015 Project Templates for Universal Windows Platform - UWPSimpleTemplate - bare bones MVVM support, UWPShellTemplate - provides a Hamburger navigation type AppShell with 4 different types of sample Views, PrismSimpleTemplate - bare bones using Prism 6 for UWP, PrismShellTemplate - same as UWPShellTemplate but using Prism 6 for UWP


[UWPTemplate](https://github.com/pablovargan/UWPTemplate)

[UWP_Application_Template](https://github.com/programmersommer/UWP_Application_Template) UWP template with pin/unpin secondary tile, share contract, rate and review and toast function

[UWP10template](https://github.com/mapaux/UWP10template) UWP template using MVVM pattern

# Composition

Note: Composition is part of the Windows API since 10586 and it should just get used. It is part of the solution to the many WPF performance complaints from Vista days. Another large issue from those days was 3D interop with DirectX and here I am not seeing any projects exploring Windows.UI.Composition and DirectX. Anyone? There is this project: [DirectCompositionDirectX12Sample](https://github.com/PJayB/DirectCompositionDirectX12Sample)

[Windows UI Dev Labs](https://github.com/Microsoft/WindowsUIDevLabs) (Previously was [Windows.UI.Composition WinRT API](https://github.com/Microsoft/composition) ) Windows UI Dev Labs the place for getting the latest code samples and demos using Windows.UI.Xaml and Windows.UI.Composition to make beautiful Universal Windows Platform applications. - Welcome to the Windows UI Dev Labs repository for the latest code samples, demos, and developer feedback for building beautiful and engaging Universal Windows Platform apps using Windows UI. The code samples and demos are targeted for developers who are interested in experimenting, building, and providing feedback on the latest flighting Windows UI APIs.

We are focused on creating a place where we can experiment, inpsire, and receive developer feedback on:
-    Flighting APIs for Windows UI
-    Testing out new UX patterns
-    Early reference implementations and prototypes
-    Inspiring demonstrations of the Windows UI API

If you are a developer getting familiar with the Windows.UI.Xaml and Windows.UI.Composition APIs, want to build beautiful UI experiences, and don't mind a few bugs here and there; then, this is the place for you. We also want to see what inspiring UX you're building and you can reach out to us on Twitter @WindowsUI. We're excited to see what you can you make with Windows UI.

We are pleased to announce that as of Windows 10 Build 10586 and SDK Version 1511 the Windows.UI.Composition API is now fully public. Many thanks to all of those who contibuted feedback to on the API during it's preview phase to make it that much better. This repository contains code samples created with the Windows.UI.Composition WinRT API. Samples contained in this repository created by the Microsoft Composition team or contributors

[UWPCompositionDemos](https://github.com/clarkezone/UWPCompositionDemos) I work on the Composition team at Microsoft that builds the Windows.UI.Composition APIs for the Universal Windows Platform. This project is where I'll be putting demos of the API's functionality when I get time :-)

[WinCompositionBehaviours](https://github.com/ScottIsAFool/WinCompositionBehaviours) A set of behaviours that use the Windows Composition APIs

[UWP audio visulization sample](https://github.com/robmikh/audiovisualization) UWP audio visulization sample. Work in progress.

[Composition Pro Toolkit](https://github.com/ratishphilip/CompositionProToolkit) Collection of Helper classes and controls (using Win2d) for Windows.UI.Composition - CompositionProToolkit is a collection of helper classes for Windows.UI.Composition. It also contains controls which can be used in UWP applications. It has dependency on the Win2D and the CompositionExpressionToolkit libraries.

[CompositionExpressionToolkit](https://github.com/ratishphilip/CompositionExpressionToolkit) A toolkit for setting the Expression in CompositionAnimation via Lambda Expressions - CompositionExpressionToolkit is a collection of Extension methods and Helper classes which make it easier to use Windows.UI.Composition features. They include methods for creating statically typed CompositionAnimation expressions, CompositionPropertySet extension methods, helper methods for creating ScopedBatchSets etc.

[CompositeHomeScreen](https://github.com/ratishphilip/CompositeHomeScreen) A mockup of iPhone home screen created using Windows.UI.Composition API - This project mainly contains a HomeScreen page which hosts the Menu and the subsequent child pages. The main constituents of the HomeScreen page can be see in the image below.


[Composition.UI](https://github.com/skendrot/Composition.UI) [Easily Create Parallax effects in Windows 10 apps](http://www.visuallylocated.com/post/2015/12/10/Easy-Parallax-effect-in-Windows-10.aspx)

[Continuity](https://github.com/JustinXinLiu/Continuity) A project that aims to provide some cool animations, transitions and controls, built on top of the new Windows Composition API.

[EffectsAndAnimationsWinComposition](https://github.com/JustinXinLiu/EffectsAndAnimationsWinComposition) Some experiments on the new effect and animation systems in Windows Composition. Please note that I could simplify things by using the TouchArea Rectangle as the container visual to host the effect visual, but I wanted to prove a point that I could use expression key frame animation to manipulate multiple elements at the same time!

![](https://camo.githubusercontent.com/44a3ce985aed3469edf86e0e7bcd1670fbdc616c/687474703a2f2f692e737461636b2e696d6775722e636f6d2f65574a62472e676966)

[StickyHeader_WindowsComposition](https://github.com/JustinXinLiu/StickyHeader_WindowsComposition) Answer to this Stack Overflow question. http://stackoverflow.com/questions/35510825/how-to-check-if-an-ui-element-has-reached-the-top-of-the-page-in-windows-phone

[PullToRefreshUWP_WindowsComposition](https://github.com/JustinXinLiu/PullToRefreshUWP_WindowsComposition) Pull to refresh with the new Windows Composition API.

[Finch](https://github.com/tomzorz/Finch) A library to help you ease into the wonders of Windows.UI.Compositon - Strongly-typed expression animations - Behaviors use effects and features with ease from XAML - Moving the needle from possible to easy with easy-to-use animation API wrapper & easy-to-use effects API wrapper

[Composition fun](https://github.com/tomzorz/Composition_fun) Fun projects with Windows.UI.Composition. Small assorted Windows.UI.Composition projects

[WinCompositionPlayground](https://github.com/WaltRitscher/WinCompositionPlayground)

[WindowsUI-Samples](https://github.com/r2d2rigo/WindowsUI-Samples) Samples and demos for Windows UI/Composition.

[WinCompositionTiltEffect](https://github.com/r2d2rigo/WinCompositionTiltEffect) A behavior for adding a tilt effect to any UWP control, implemented using Windows Composition.

[CompositionAnimations](https://github.com/Sergio0694/UICompositionAnimations) A wrapper PCL for the Windows.UI.Composion animations

[CompositionAnimationsDemo](https://github.com/renewal-wu/CompositionAnimationsDemo)

[CompositionEntranceAnimationExample](https://github.com/tracker086/CompositionEntranceAnimationExample) no desc.

[CarouselView](https://github.com/pengzhxyz/CarouselView) An UWP carousel control supporting looping and based on composition api
-    It supports infinite looping scrolling
-    AutoSwitch supporting
-    It could show 3 pictures at the same time, rather than filpview which only shows one picture
-    Responsable to the container size
-    Touch or mouse wheel
-    Thanks to the Composition API!

[CompositionGridView](https://github.com/pnp0a03/CompositionGridView) no desc.

[UWP-Composition-Radial-Gauge](https://github.com/XamlBrewer/UWP-Composition-Radial-Gauge) A XAML Radial Gauge Custom Control for UWP 

[UWP-Composition-Rating-Control](https://github.com/XamlBrewer/UWP-Composition-Rating-Control) A UWP Rating Control drawn by the Composition API.

[UWP-Composition-API-Clock](https://github.com/XamlBrewer/UWP-Composition-API-Clock) Demonstrates using the Composition API in a Universal Windows Platform 

[UWP-Composition-Effects-Sample](https://github.com/XamlBrewer/UWP-Composition-Effects-Sample) An UWP app that illustrates some of the Composition API effects:
- [Hue Rotation](https://xamlbrewer.wordpress.com/2016/04/08/uwp-composition-effects-hue-rotation/)
- [Temperature and Tint](https://xamlbrewer.wordpress.com/2016/04/19/uwp-composition-effects-temperature-and-tint/)
- [Effect chaining](https://xamlbrewer.wordpress.com/2016/05/15/uwp-composition-effects-chaining/)


[CompositionHelper](https://github.com/higankanshi/CompositionHelper) CompositionHelper for UWP Composition API. Now we support all animation of Composition API. You can build composition animations by fluent interface. You can use XAML to set UIElement's Visual composition properties. We found there are some Airspace issue between Composition API visual tree and XAML visual tree, so we remove shadow effect, but you can still find those codes in early Commit.

[CompositionAPI](https://github.com/agangal/CompositionAPI)

[Composition Animation Toolkit](https://github.com/aL3891/CompositionAnimationToolkit) The Composition animation toolkit is a set of tools that is ment to make working with animations in the Windows.Ui.Composition libraries easier. Specifically, it allows users to write animation expressions using statically typed lambda expressions instead of strings. It also has features to make working with property sets easier, such as providing a wrapper that user classes can derive from to make static properties for the contents in the property set, as well as generating property sets from any other class, including anonymous classes.

[CompositionImageLoader](https://github.com/robmikh/compositionimageloader) An image loader to use with the Windows.UI.Composition api based on Win2D and written with C#.

[CompositionBlendEffect](https://github.com/cyrilcathala/CompositionBlendEffect) Simple blend effect with Windows.UI.Composition

[UICompositionExploration](https://github.com/a7an/UICompositionExploration) Exploration of UI Composition or something like that could be hypothesized when there is yet another project with no description. 



# Frameworks

[MVVM-Sidekick](https://github.com/waynebaby/MVVM-Sidekick) A Modern light-weight MVVM framework based on RX and Await

[MugenMvvmToolkit](https://github.com/MugenMvvmToolkit/MugenMvvmToolkit) Mugen MVVM Toolkit makes it easier to develop cross-platform application using the Model-View-ViewModel design pattern. The Mugen MVVM Toolkit makes extensive use of Portable Class Libraries to provide maintainable cross platform C# native applications.

[mvvmlight](https://github.com/timdetering/mvvmlight) Git mirror of GalaSoft MVVM Light Toolkit (https://mvvmlight.codeplex.com/)

[Prism](https://github.com/PrismLibrary/Prism) Prism is a framework for building loosely coupled, maintainable, and testable XAML applications in WPF, Windows 10 UWP, and Xamarin Forms.

[Caliburn.Micro](https://github.com/Caliburn-Micro/Caliburn.Micro) A small, yet powerful framework, designed for building applications across all XAML platforms. Its strong support for MV* patterns will enable you to build your solution quickly, without the need to sacrifice code quality or testability. http://caliburnmicro.com/

[Okra App Framework](https://github.com/OkraFramework/Okra.Core) The Okra App Framework is designed to support the development of .Net Windows Store applications, in particular those following the MVVM pattern. http://okraframework.github.io -  [Okra.Platform.UniversalWindows](https://github.com/OkraFramework/Okra.Platform.UniversalWindows) provides platform specific code for developing Okra App Framework based UWP applications

[Crystal](https://github.com/Amrykid/Crystal) My secret sauce: A UWP Application development framework. Batteries required! Crystal is a UWP application development framework I use for my own projects. It essentially a way for me to get started quickly and not have to get my hands dirty. Batteries are not included. Use at your own risk!

[Framework](https://github.com/RavinduL/Framework) A simple framework for developing UWP apps. [Docs](https://github.com/RavinduL/Framework/wiki)

# Controls

[UWPCommunityToolkit](https://github.com/Microsoft/UWPCommunityToolkit) Updated to 1.1 :sun_with_face: Microsoft has assembled about 12 Controls, many of them from other projects on this list, and other misc helper libs for UWP programming. At the moment, it seems like it is far less ambitious in scope than their Template 10 project, yet for some reason they have heavily promoted this Community Toolkit both with press releases and featuring on their [Developer website](https://developer.microsoft.com/en-us/windows/samples). The [UWPCommunityToolkit-docs](https://github.com/Microsoft/UWPCommunityToolkit-docs) is a separate GitHub project which feeds this [Microsoft.com Windows Dev site](https://developer.microsoft.com/en-us/windows/uwp-community-toolkit). There is a [Sample App in Windows Store](https://www.microsoft.com/store/apps/9nblggh4tlcq) that allows you to see exactly what is in the kit. 

There is no mention of any Blend specific features or add-ons but there is an instruction on [how to add the kit to the VS 2015 Designer Toolbox](https://developer.microsoft.com/en-us/windows/uwp-community-toolkit/toolbox). Actually, Blend does a great job of picking up any controls referenced in the project and no installation is needed. Please keep Blend alive and get the add-ons working right for Blend!

For some reason Windows Composition is partially missing in action for this kit. IMO, both Windows Composition and Win2D are unique Microsoft UWP technologies that can make the platform exciting and are natural candidates for this Microsoft showcase. Part of the problem is that Anniversary (14393) is where Composition starts to light up and show its significance and the Community Toolkit wants to support the previous Windows 10 version as well.

#### Controls:
-    AdaptiveGridView
-    BladeControl
-    DropShadowPanel
-    GridSplitter
-    HamburgerMenu
-    HeaderedTextBlock
-    ImageEx
-    PullToRefreshListView
-    RadialGauge
-    RangeSelector
-    RotatorTile
-    SlideableListItem
    
#### Animations

-    Blur
-    Offset
-    Fade
-    Rotate
-    Scale
-    FadeHeader
    
#### Code Helpers

-    Colors
-    Connection
-    Converters
-    ImageCache
-    Incremental Loading Collection
-    Object Storage
-    StorageFiles
-    Streams
-    VisualTreeExtensions
-    WeakEventListener


#### Services

-    Bing
-    Facebook
-    LinkedIn
-    Microsoft Graph
-    Twitter

#### Notifications

-    Tiles
-    Toasts

[Windows App Studio Libraries](https://github.com/wasteam/waslibs) This repository contains the source code of the libraries used by Windows App Studio in the generated apps. There are three libraries: utility classes to create XAML applications, all the data sources available in Windows App Studio apps, and XAML controls for Windows 10 apps only.

#### Layout Controls

-    ResponsiveGridView
-    Pivorama
-    VariableSizedGrid
-    Carousel
-    SliderView
-    SectionList
-    SplitterCard

#### Foundation Controls

-    HtmlBlock
-    VisualBreakpoints
-    ImageEx
-    GifControl
-    VirtualBox
-    RelativeBox
-    RelativeBox and VirtualBox
-    SearchBox
-    InfiniteScroll

#### Labs Controls

-    ResponsiveGridView
-    Accordion
-    SlideShow
-    ShapeImage
-    AutoHide
-    Mosaic
    
#### App Services

-    Navigation
-    AppCache

#### Utilities

-    ErrorNotification
-    ActionsCommandBar
-    AnimationExtensions
-    Converters

#### Data Providers Library

-    Facebook
-    Twitter
-    Flickr
-    YouTube
-    WordPress
-    Rss
-    Bing
-    LocalStorage
-    REST API

[WinRTXamlToolkit](https://github.com/xyzzer/WinRTXamlToolkit) A set of controls, extensions and helper classes for Windows Runtime XAML applications.

#### Controls

-    AlternativeFrame, AlternativePage - support asynchronous page transitions and preloading pages so when navigation is initiated - all content might already be loaded. Includes 4 built-in transitions: dissolve, flip, push, wipe. You can add new ones yourself.
-    AnimatingContainer - a container control that will animate its contents rotating or zooming in/out, eg. to make them feel more alive.
-    AutoCompleteTextBox - a TextBox with dictionary-based autocompletion support by fex with keyboard support added by yours truly.
-    CameraCaptureControl - supports displaying camera preview, capturing photos and videos, cycling between existing video capture devices, setting preference to Front/Back panel camera, etc.
-    CascadingTextBlock - a TextBlock replacement that animates the individual letters in a cascade - fading in while falling down into position, then optionally fading out while falling down from the standard position.
-    Chart - Silverlight Toolkit's Chart control ported by Mahmoud Moussa (ZeeMoussa on CodePlex) and merged from his Windows 8 Toolkit - Charts and More project. Supports pie charts, bar charts, scatter charts, etc.
-    CountdownControl - a movie-style control that animates a ring-slice shape while counting down seconds - e.g. to take a picture with a camera after a given number of seconds (supports async/await).
-    CustomAppBar - a custom implementation of the AppBar that automatically handles the three gestures to switch IsOpen (WinKey+Z, Right-Click, EdgeGesture), adds a CanOpen property, so you can prevent it from opening and opens/hides with a sliding animation when placed anywhere in the app, so you can layer content on top of it. Also features CanDismiss property to force the app bar to stay open in some situations, CanOpenInSnappedView which allows to block the app bar from showing up when the app is in the snapped view.
-    CustomGridSplitter - a custom implementation of a GridSplitter as a templated control.
-    DelayedLoadControl - given a content/DataTemplate - loads the contents after a given amount of time - e.g. to allow for staged loading of contents on screen.
-    ImageButton - a custom Button control that takes one to three images to be used to represent different states of the button (normal/hover/pressed/disabled) as well as ways for the button to render all 4 states with just one or two images.
-    ImageToggleButton - custom ToggleButton control, that like ImageButton - helps create buttons based on button state images using from 1 to 8 different state images and generating other state images with some simple image processing.
-    InputDialog - a custom/templated dialog control that takes text input.
-    ListItemButton - a simple button control with Click event and Command property to be used inside of list controls (the standard button steals pointer capture from the List/Grid~Items so they can't be selected.
-    NumericUpDown - allows to display and manipulate a number using text input, +/- buttons or Blend-like swipe-manipulations
-    PieSlice - a pie slice path/shape given StartAngle, EndAngle and Radius.
-    RingSlice - a pie slice path/shape given StartAngle, EndAngle, Radius and InnerRadius.
-    TreeView - traditional tree view control ported from Silverlight Toolkit. Has separate touch and mouse themes.
-    ToolWindow - a window content control that snaps/docks to edges if the screen or parent control.
-    WatermarkTextBox - TextBox control with a watermark. Set WatermarkText to change the watermark prompt, change WatermarkStyle to change the style of the watermark TextBlock.
-    WebBrowser - a templated control with a WebView + address bar, title bar, backstack navigation, favicon. work in progress (visual states are a bit messed up), but might be helpful as a starting point
-    WrapPanel (ported from Silverlight Toolkit) - used for layout of child items in wrapping rows or columns - similar to the way text wraps on a page. Different than VariableSizedWrapGrid since it supports items of varying size and auto-sized rows or columns, but it is not a grid and so it does not explicitly support items spanning multiple cells without the use of negative margins.

#### Controls.Extensions

-    AnimationHelper - two attached properties - Storyboard and IsPlaying. Allows to easily control Storyboard playback from a view model (note limitation - a single storyboard per control).
-    AppBarExtensions.HideWhenSnapped - allows to make the AppBar automatically hide when the app goes to the snapped view.
-    ContentControlExtensions.FadeTransitioningContentTemplate - allows to change content template with a fade out/fade in transition.
-    ControlExtensions.Cursor - enables setting a mouse cursor to show when hovering over a control.
-    FrameworkElementExtensions.ClipToBounds - automatically updates the Clip property to clip the contents of the element to its bounds.
-    ImageExtensions.FadeInOnLoaded/.Source - allows to specify an image source such that the image fades in smoothly when the image source is loaded.
-    ListBoxExtensions./ListViewExtensions
-        BindableSelection - allows a two-way binding of the SelectedItems collection on the Selector/list controls.
-        ItemToBringIntoView - allows to control which item should be visible through a view model binding without changing the selected item itself.
-    ManipulationInertiaStartingRoutedEventArgsExtensions - adds extensions to the arguments of the ManipulationInertiaStarting event that calculate flick ballistics - help determine and control where and when an inertial manipulation will end so you can make your flicks always end where you want them to! It's the basis of the ToolWindow behavior where a flicked window always quickly and smoothly snaps to the side of the screen.
-    RichTextBlockExtensions
-        PlainText - attached property that allows to easily single-way-bind plain text to a RichTextBlock (not really that useful other than for visualizing RichTextBlock styles in the sample app provided).
-        LinkedHtmlFragment - attached property that allows to easily single-way-bind plain text with HTML links (anchor tags) to a RichTextBlock to automatically generate links. Extension methods like SetLinkedHtmlFragment() and AppendLink() are also available.
-    ScrollViewerExtensions.ScrollToHorizontalOffsetWithAnimation(), .ScrollToVerticalOffsetWithAnimation() - provide a way to scroll a ScrollViewer to specified offset with an animation.
-    TextBlockExtensions/GetCharacterRect() - an extension method that returns a rectangle that holds a character at a given index in the TextBlock.
-    TextBoxValidationExtensions - extensions that allow to specify the Format of the requested Text input as well as brushes to use to highlight a TextBox with valid or invalid Text.
-    ViewboxExtensions.GetChildScaleX()/GetChildScaleY() - return the effective scale of the Viewbox Child.
-    VisualTreeHelperExtensions - provides a set of extension methods that enumerate visual tree ascendants/descendants of a given control - making it easy to do these operations with LINQ as well as simple ways to list controls of a given type or find the first control of a given type searching up or down the visual tree.
-    WebViewExtensions - extensions to get currently loaded page address, title, favicon, head tag's inner HTML.
#### Imaging Extensions

-    BitmapImageLoadExtensions - extensions to simplify loading BitmapImages based on StorageFile or file name
-    ColorExtensions - Conversions between pixels and pixel buffer types of byte, int and Color
-    IBufferExtensions - Adds a GetPixels() extension method to the PixelBuffer property of a WriteableBitmap that reads in the buffer to a byte array and exposes an indexer compatible to the one of the Pixels property in Silverlight's WriteableBitmap
-    WriteableBitmap~ - a set of extension methods for a WriteableBitmap
-        WriteableBitmapSaveExtensions - support for loading and saving the bitmap to/from files
-        WriteableBitmapBlitBlockExtensions - support for quick blitting of a full-width section of a bitmap to another bitmap of same width
-        WriteableBitmapCopyExtensions - support creating a copy of a WriteableBitmap
-        WriteableBitmapCropExtensions - support for creating a cropped version of a WriteableBitmap
-        WriteableBitmapDarkenExtension - performs image processing to darken the pixels of the WriteableBitmap.
-        WriteableBitmapFloodFillExtensions - support for flood-filling a region of a WriteableBitmap - either limited by an outline color or by replacing a given color - usually a color at the starting position or colors similar to it
-        WriteableBitmapFromBitmapImageExtension - allows to create a WriteableBitmap from a BitmapImage assuming the BitmapImage is installed with the application.
-        WriteableBitmapGrayscaleExtension - performs image processing to make the pixels of the WriteableBitmap (more) grayscale.
-        WriteableBitmapLightenExtension - performs image processing to lighten the pixels of the WriteableBitmap.

#### IO helpers

-    ScaledImageFile.Get() - Used to retrieve a StorageFile that uses qualifiers in the naming convention.
-    StorageFileExtensions.GetSize()/.GetSizeString() - allow to get the size of a file and its string representation (automatically converting from bytes to kB, MB, GB, TB)
-    StorageFolderExtensions
        .ContainsFile() - returns a value that states whether a file with specific name exists in the folder
        .CreateTempFile() - creates a temporary file
        .CreateTempFileName() - returns an unused, unique file name for a temporary file
-    StringIOExtensions - allows to easily read or write a string from/to file in a single call
-    Serialization
-        JsonSerialization - allows to serialize a properly DataContract-annotated object to a JSON string or file or deserialize an existing one.
-        XmlSerialization - allows to serialize a properly DataContract- or XmlSerializer-annotated object to a XML string or file or deserialize an existing one.

[MyToolkit](https://github.com/MyToolkit/MyToolkit) MyToolkit for .NET http://mytoolkit.io MyToolkit is a set of .NET libraries containing lots of useful classes for various .NET platforms like UWP/WinRT (Universal Windows Apps), Windows Phone and WPF. The goal is to provide missing or replace existing classes to support the development of high-quality Windows and Windows Phone applications. For example, the library provides often used MVVM infrastructure classes, missing UI controls, IoC classes, additional LINQ extension methods and much more.

- MVVM classes (RelayCommand, ViewModelBase, ObservableObject, Messenger) in portable class library
- Networking classes: HTTP with GZIP support, WakeOnLan
- XAML controls and converters, e.g. MtPivot, DataGrid for WinRT/UWP and Hamburger for UWP
- Improved paging classes for Universal Windows Apps (UWP), Windows Phone and Windows 8 apps
- Additional collections like ObservableDictionary, MtObservableCollection or ObservableCollectionView 

#### Controls
- 	AppBarButton.cs 	
-	AppBarToggleButton.cs 	
-	ColorChooser.cs 	
-	DataTemplateSelector.cs 	
-	FadingImage.cs 	
-	GenericDataTemplateSelector.cs 	
-	GridControl.cs 	
-	HorizontalHtmlGenerator.cs 	
-	ImageButton.cs 
-	ItemsWrapGridExtensions.cs 
-	LongListSelector.cs 	
-	LongListView.cs 	
-	MenuListBox.cs 	
-	MtGridView.cs 	
-	MtItemsControl.cs 	
-	MtListBox.cs 	
-	MtListView.cs 	
-	MtPivot.cs 	
-	MtPivotItem.cs 	
-	NavigationGridView.cs 	
-	NavigationList.cs 	
-	NavigationListEventArgs.cs 
-	NavigationListView.cs 	
-	OrientedSize.cs 	
-	PanAndZoomImage.cs 	
-	PanAndZoomViewer.cs 	
-	PivotExtensions.cs 	
-	PrepareContainerForItemEventArgs.cs 	
-	RolloverButton.cs 	
-	ScrollableItemsControl.cs 	
-	SuppressTappedPresenter.cs 	
-	TextButton.cs 	
-	UniformGrid.cs 	
-	WatermarkedTextBox.cs 	
-	WrapPanel.cs

[Composition Pro Toolkit](https://github.com/ratishphilip/CompositionProToolkit) Collection of Helper classes and controls (using Win2d) for Windows.UI.Composition - CompositionProToolkit is a collection of helper classes for Windows.UI.Composition. It also contains controls which can be used in UWP applications. It has dependency on the Win2D and the CompositionExpressionToolkit libraries.

#### Controls:

- Fluid Progress Ring
- Fluid Wrap Panel
- Fluid Banner
- Image Frame

[Continuity](https://github.com/JustinXinLiu/Continuity) A project that aims to provide some cool animations, transitions and controls, built on top of the new Windows Composition API.

#### Controls:
- Tab


[CarouselView](https://github.com/pengzhxyz/CarouselView) An UWP carousel control supporting looping and based on composition api
-    It supports infinite looping scrolling
-    AutoSwitch supporting
-    It could show 3 pictures at the same time, rather than filpview which only shows one picture
-    Responsable to the container size
-    Touch or mouse wheel
-    Thanks to the Composition API!

[UWP-Composition-Rating-Control](https://github.com/XamlBrewer/UWP-Composition-Rating-Control) A UWP Rating Control drawn by the Composition API. There's a blog post explaining the code right here: https://xamlbrewer.wordpress.com/2016/07/11/building-a-uwp-rating-control-using-xaml-and-the-composition-api/ - Comes with the following dependency properties:
-    Maximum (int): number of stars, maximum score
-    StepFrequency (double): rounding interval, a percentage (e.g. 0.25)
-    Value (double): current value (from 0 to Maximum)
-    ItemHeight (int): height (and width) of each image in device independent pixels
-    ImagePadding (int): pixels between images
-   FilledImage (uri): path to the filled image
-    EmptyImage (uri): path to the empty image
-    IsInteractive (bool): whether or not the control responds to user input (tapping or sliding)
Behavior:
- Tap on an image to apply the integral value
- Slide horizontally over the control to decrease and increase value with StepFrequency

[Marduk.Controls](https://github.com/ProjectMarduk/Marduk.Controls) Controls library for Universal Windows.([Nuget](https://www.nuget.org/packages/Marduk.Controls/))

- PhotowallView A stand alone photo wall layout control with virtualizing capability. 
- WaterfallFlowView A stand alone waterfall flow layout controls with virtualizing capability. 

![](https://cloud.githubusercontent.com/assets/9367842/17103395/aeb31994-52b0-11e6-85a0-810188084535.gif)

- UI Virtualizing Both of PhotowallView and WaterfallFlowView support UI virtualizing which enables the system to render only the visible items inside the viewport.
- Incremental Loading Just make your ItemSource inherits form Windows.UI.Xaml.Data.ISupportIncrementalLoading then the control would do the rest.
- Item Tapped Event Hooking up to the ItemTapped event with PhotowallView or WaterfallFlowView to get notified when an item was tapped.
- Easy Styling/ Comprehensive Visual States/ Multiselection Easily styling the appearence of PhotowallView and WaterfallFlowView with the preset visual states such as "IsSelected" and "NotSelected" etc.
- High Performance for Random Insert, Remove and Change  Freely random insert, remove or change an item, even it's been virtualized.
- High Performance for Resizing You can use Marduk.Controls.OrientedVirtualizingPanel.Resizer to optimize resize behavior

[CompositionGridView](https://github.com/pnp0a03/CompositionGridView) no desc.

[UWP-Composition-Radial-Gauge](https://github.com/XamlBrewer/UWP-Composition-Radial-Gauge) A XAML Radial Gauge Custom Control for UWP that is partially drawn by the Composition API. It uses the release version of Composition API, so this requires Requires Visual Studio 2015 update 1 and Windows 10 10586 SDK on your side. A blog post that explains the code is right here: https://xamlbrewer.wordpress.com/2016/01/23/building-a-custom-uwp-control-with-xaml-and-the-composition-api/.

[UWP-Composition-API-Clock](https://github.com/XamlBrewer/UWP-Composition-API-Clock) Demonstrates using the Composition API in a Universal Windows Platform XAML control.Requires Visual Studio 2015 update 1, and Windows 10 10586 SDK. Contains a copy of Microsoft.UI.Composition.Toolkit that is maintained here: https://github.com/Microsoft/composition. A blog post explaining the code is here: https://xamlbrewer.wordpress.com/2016/01/04/using-the-composition-api-in-uwp-apps/.



[UniversalMarkdown](https://github.com/QuinnDamerell/UniversalMarkdown) A markdown parsing and rendering library for C# and Windows Universal Apps http://baconit.quinndamerell.com/ Universal Markdown is your one-stop-shop for all of your markdown needs in C#. Universal markdown was built for the open source reddit app Baconit, but hopefully it will be adopted by others and improved by the community. 

[IpatovUWP](https://github.com/Opiumtm/IpatovUWP) UWP common use helper libraries such as util code for DataBinding. New, is a Markup rendering engine based on Direct2D instead of XAML tree manipulations. [Nuget: Ipatov.MarkupRender](https://www.nuget.org/packages/Ipatov.MarkupRender/) First public release is very simplistic and not feature rich, but most important feature of this library is very high performance.

[WinRT-StandardDateFormatPicker](https://github.com/ignacy130/WinRT-StandardDateFormatPicker) Simple control based on ComboBoxes to pick date in common in Europe and most of the world format dd-mm-yyyy. Wiki: https://github.com/ignacy130/WinRT-StandardDateFormatPicker/wiki

[RichTextBlock.Html2Xaml](https://github.com/MacawNL/WinRT-RichTextBlock.Html2Xaml) The WinRT RichTextBlock control serves to display read-only rich formatted text. However, it supports a limited subset of XAML, and no HTML. In scenario's where you want to display a field that contains HTML rich formatted text (e.g. when you have clients on multiple platforms, such as web, WinRT, iOS and Android), this package offers an alternative to using an embedded browser control. Using a browser control impacts performance and limits the UI experience (e.g. the WebView control does not support transparency). RichTextBlock.Html2Xaml adds an Html extension property to RichTextBlock controls, that you can set (or data bind) to a string containing an Html snippet.

[Mntone WinRT Library](https://github.com/mntone/WinRtLibrary) This is my useful library for UWP and Windows Store app - UI.Xaml.Controls - TypedDataTemplateSelector - VisualTreeHelper2

[UWP-master](https://github.com/zmtzawqlp/UWP-master)Some controls such as FlexGrid, DataGrid, Charts etc.

[Radial Menu](https://github.com/CatalystCode/radial-menu) A Radial Menu for Windows UWP Applications, as made popular by the first versions of the modern OneNote App for Windows. Create radial menus floating op top of your application. The control supports variable numbers of buttons, toggle & radio buttons, a selector for long lists, and a fancy metered menu for intuitive selection of numbers.
![](https://github.com/CatalystCode/radial-menu/raw/CaseStudyDemo/gif.gif)

[UWP-Radial-Gauge-Sample](https://github.com/XamlBrewer/UWP-Radial-Gauge-Sample) Demonstrates using the WinRT XAML Toolkit Radial Gauge on the Universal Windows Platform

[UWP-Composition-Radial-Gauge](https://github.com/XamlBrewer/UWP-Composition-Radial-Gauge) A XAML Radial Gauge Custom Control for UWP that is partially drawn by the Composition API. A blog post that explains the code is right here: https://xamlbrewer.wordpress.com/2016/01/23/building-a-custom-uwp-control-with-xaml-and-the-composition-api/. There's a newer version of this control in the UWP Community Toolkit: https://github.com/Microsoft/UWPCommunityToolkit.

[RadialSlider](https://github.com/galazzo/RadialSlider) A radial Slider for Windows 10 Universal Windows Platform (UWP)

[SplitViewMenuUWP](https://github.com/deanchalk/SplitViewMenuUWP) A custom control for a split view (hamburger) left menu for windows 10 univeral apps

[UWP-UniformGrid-Control](https://github.com/rickapps/UWP-UniformGrid-Control) The missing UniformGrid control from WPF ported to UWP

[ButterSwitch](https://github.com/validvoid/ButterSwitch) A butter-like style toggleswitch control for UWP apps. Including a style for built-in toggleswitch control and a standalone toggleswtich templated custom control.

[ExpanderUWP](https://github.com/deanchalk/ExpanderUWP) Expander Control for Microsoft UWP

[Kimono](https://github.com/Amrykid/Kimono) A Windows 10 UWP (.NET) library with a set of UI controls

[WinUX-UWP-Toolkit](https://github.com/jamesmcroft/WinUX-UWP-Toolkit) A collection of core XAML controls and extensions to use in your personal universal Windows apps http://jamescroft.co.uk/blog/uwp/introducing-croft-core-for-universal-windows-apps/

[comet](https://github.com/nmetulev/comet) Note: this project formed the starter seed of the Microsoft Community Toolkit (see above) so AFAIK it is no longer maintained. Previously: Universal Windows Platform (UWP) toolkit library. Contains controls for creating great user experiences for Universal Windows Applications



[Naylah.Toolkit.UWP](https://github.com/NaylahProject/Naylah.Toolkit.UWP) Naylah SDK for Universal Windows Plataform http://naylahproject.github.io/Naylah.UWP/ Contain useful libraries, controls, helpers, architecture, etc. The intent is create a community for developers focusing in deliver better-beatiful apps. To create next generation of apps.

[Coding4FunToolkit](https://github.com/Coding4FunProjects/Coding4FunToolkit) This is where Coding4Fun will house all our cool controls and tools that we come up with

[UwpProjects](https://github.com/LanceMcCarthy/UwpProjects) A set of UWP controls and utilities. 
    BusyIndicators in UwpHelpers.Controls.BusyIndicators (cool custom busy indicator)
    AdaptiveGridView in UwpHelpers.Controls.ListControls (maintains aspect ratio of items as it scales for column width)
    BlurElementAsync in UwpHelpers.Examples.Helpers (converts any UIElement into a blurred BitmapImage)
    IncrementalLoadingCollection in UwpHelpers.Controls.Common (demo in Examples)
    NetworkImage in UwpHelpers.Controls.ImageControls (an Image control that shows download progress)

[WinRT_Calendar](https://github.com/bak301/WinRT_Calendar)

[FABExt.UWP](https://github.com/JuniperPhoton/FABExt.UWP) A FAB-like control on Windows.

[QuickReturnHeader](https://github.com/pdehne/QuickReturnHeader) Universal Windows Platform (UWP) quick return header control to be used with ListViews - Add the QuickReturnHeader class to your project. Then define a regular ListView and add a QuickReturnHeader to its header. Make sure to tell the header which ListView it belongs to using the TargetListView property:

[Font-Awesome-WPF/UWP](https://github.com/charri/Font-Awesome-WPF)  WPF & UWP controls for the iconic font and CSS toolkit Font Awesome. Font Awesome: http://fortawesome.github.io/Font-Awesome/ UWP glyph control for the iconic font and CSS toolkit Font Awesome. [UWP Readme](https://github.com/charri/Font-Awesome-WPF/blob/master/README-UWP.md)

[SwipeListView](https://github.com/FrayxRulez/SwipeListView) A ListView with swipe handling like the one in new Outlook Mail app for Windows 10.

[UWPBox](https://github.com/ruffin--/UWPBox) Fixing TextBox wackiness for UWP applications

[LocalNotifications](https://github.com/RavinduL/LocalNotifications) Local (in-app) notifications for UWP applications.
![](https://github.com/RavinduL/LocalNotifications/raw/master/images/demo.gif)

# UI
[ReactiveUI](https://github.com/reactiveui/ReactiveUI) A MVVM framework that integrates with the Reactive Extensions for .NET to create elegant, testable User Interfaces that run on any mobile or desktop platform. Supports Xamarin.iOS, Xamarin.Android, Xamarin.Mac, Xamarin Forms, WPF, Windows Forms, Windows Phone 8, Windows Store and Universal Windows Platform (UWP). http://www.reactiveui.net

[userdialogs](https://github.com/aritchie/userdialogs) A cross platform library that allows you to call for standard user dialogs from a shared/portable library, Actionsheets, alerts, confirmations, loading, login, progress, prompt, toast... async just for fun. Supports Android, iOS, Windows Phone 8.0 (silverlight), and Unified Windows Platform (UWP, UAP)

[BlendrocksToolkit](https://github.com/deanihansen/BlendrocksToolkit) Windows UWP toolkit that which enabled insanely cool page transitions and easier navigation and app handling.

[Monolith](https://github.com/ThatLousyGuy/Monolith) Monolith is a Windows library that lets you create animations in codebehind in a fluent, somewhat straightforward manner. It's a wrapper around the Windows.UI.Xaml.Media.Animation library that removes as much of the setup as possible. (Thanks to [Awesome UWP resources list](https://github.com/tomzorz/awesome-uwp) for the head's up on this interesting project.

[MonolithUWP](https://github.com/JuniperPhoton/MonolithUWP) A UWP version of Monolith,which is a Windows library that lets you create animations in codebehind in a fluent, somewhat straightforward manner.

[WindowsStateTriggers](https://github.com/dotMorten/WindowsStateTriggers) A collection of custom visual state triggers


# Libs UWP

Libraries that may support UWP specific features.

[UWPHelper](https://github.com/bramborman/UWPHelper) A set of useful UWP tools such as converters, triggers and helpers.

[Wallace.UWP.Helpers](https://github.com/miao17game/Wallace.UWP.Helpers)


[Groves](https://github.com/tomzorz/Groves) A UWP library by the author of the [Awesome UWP resources list](https://github.com/tomzorz/awesome-uwp) 

[YAWL.Composition](https://github.com/YAWL/YAWL.Composition) Composable building blocks for MVVM based Windows 10 applications

[observable-vector](https://github.com/jamesqo/observable-vector) A no-frills implementation of IObservableVector for Windows 10 apps.

[Shims.Xaml](https://github.com/jamesqo/Shims.Xaml) Easily create libraries that work on both WPF and Windows 10.

[XamlBehaviors](https://github.com/Microsoft/XamlBehaviors) This is the official home for XAML Behaviors on GitHub. XAML Behaviors is an easy-to-use means of adding common and reusable interactivity to your Windows UWP applications with minimal code. It is available for both native and managed applications.

[Portable.Xaml](https://github.com/cwensley/Portable.Xaml) Portable .NET library for reading/writing xaml files. This is intended to be used to read Xaml on desktop, mobile, and CoreCLR platforms.

[typed-xaml](https://github.com/jamesqo/typed-xaml) Advanced generics support for WPF and Windows 10.

[uwp-chrome](https://github.com/RReverser/uwp-chrome) Experimental chrome API shim for Universal Windows Platform (UWP / WinRT)

[UWP-Helpers](https://github.com/EdiWang/UWP-Helpers) Helpers and Utils for UWP Projects

[Kulman.UWP](https://github.com/igorkulman/Kulman.UWP) Collection of utilities and services for UWP apps



[Cimbalino-Toolkit](https://github.com/Cimbalino/Cimbalino-Toolkit) Cimbalino Toolkit http://cimbalino.org Cimbalino Toolkit is a set of useful and powerful tools that will help you build your Windows Platform applications.

[cadru](https://github.com/scottdorman/cadru) A Microsoft .NET Framework toolkit http://scottdorman.github.io/cadru Cadru is a utility framework containing new APIs and extensions to the core .NET Framework to help complete your developer toolbox. It is designed to be portable first, which means that the majority of the library is available as a Portable Class Library (PCL) 

[Windows-task-snippets](https://github.com/Microsoft/Windows-task-snippets) This repo collects snippets of ready-to-use code that accomplish small but useful tasks of interest to Universal Windows Platform (UWP) app developers. These snippets represent simple solutions to common problems, and simple recipes to help you implement new app features. 

[UWP-Networking-Essentials](https://github.com/SvenEV/UWP-Networking-Essentials) Simple and lightweight networking (including RPC) for Universal Windows Platform apps

[ComposableAdaptiveTriggerDemo](https://github.com/LocalJoost/ComposableAdaptiveTriggerDemo) Demo of a AdaptiveTrigger that works with a StateTrigger inside a CompositeStateTrigger from WindowsStateTriggers

[YAWL.Common](https://github.com/YAWL/YAWL.Common) Common library for all new Windows Phone/Store/UWP/Mobile and Xamarin applications

[WinRT.IncrementalLoadingCollection](https://github.com/AhmedMabrouck/WinRT.IncrementalLoadingCollection) A Windows Runtime custom collection that supports observability and incremental loading out of the box.

[inflatable-toolkit](https://github.com/inflatablefriends/inflatable-toolkit) Stuff we use a lot in WinRT apps

[bigint-winrt](https://github.com/robpaveza/bigint-winrt) A Windows Runtime API for big integers. The source BigInteger implementation is forked from https://github.com/kurmasz/bigint which is based on the bigint library by Matt McCutchen. 

[MetroLog](https://github.com/onovotny/MetroLog) MetroLog is a lightweight logging framework designed for Windows Store and Windows Phone 8 apps. Although the API is based on NLog and log4net, the intention is that it's a very basic logging system. 
The need for it to be basic comes from the fact that the Windows Store apps API surface area intentionally limited for very specific applications. This project came out of the fact that porting NLog to Windows Store apps is difficult because of it's incredibly rich feature set, most of which is not workable in Windows Store apps.

[WinRTTimeZones](https://github.com/onovotny/WinRTTimeZones) Simple Time Zone conversion for WinRT, Windows Store and Windows Phone 8 apps

[SLARToolkit - Silverlight and Windows Phone Augmented Reality Toolkit](https://github.com/amoldeshpande/slartoolkit) UWP adaptation from [CodePlex](https://slartoolkit.codeplex.com/) This is an incomplete port of SLArToolkit for Windows 10 UWP. 
![](http://download-codeplex.sec.s-msft.com/Download?ProjectName=SLARToolkit&DownloadId=233583)
I have added the capability to capture video for UWP apps, which was the major hurdle. Beginners Guide version for Windows 10 almost works, except for camera rotation being off by 90 degrees. 

[ModuloLib](https://github.com/amoldeshpande/ModuloLib) This is a C# Windows 10 UWP class library for the Modulo platform (http://www.modulo.co) It contains basic serial communication as well as classes for interaction with the Display, Knob and Joystick modulos. (Modulo is a set of tiny modular circuit boards that you can assemble to build powerful programmable electronics without needing to design and assemble circuits from scratch.)

[UwpLib](https://github.com/romagny13/UwpLib) Misc UWP 

[JP.Utils.UWP](https://github.com/JuniperPhoton/JP.Utils.UWP) 

[Aura.Net](https://github.com/Lukasss93/Aura.Net) Utilities Class Library for Windows Phone 8.1 RT & UWP

# Libs to access an API

[DeviantartApi Library](https://github.com/Mr1Penguin/DeviantartApi) DeviantartApi Library in C# for UWP, Win8.1, WinPhone8.1,. NET 4.5+, ASP.NET Core 1.0

[Bex](https://github.com/ScottIsAFool/Bex) A PCL for accessing the MS Health Web APIs. For usage and an overview, please go to http://metronuggets.com/2015/07/10/introducing-bex-a-pcl-library-for-the-ms-health-apis/

[Discord-UWP](https://github.com/gantonious/Discord-UWP) A Discord wrapper in C# compatible with UWP.

# Libs General

Libraries that are compatible with UWP but don't provide UWP specific feature support.




[Shim](https://github.com/cureos/shim) Shim provides reduced or dummy implementations of .NET Framework types that are currently not represented in PCL, thereby expanding the ability to create Portable Class Libraries from legacy code.

[InternalContainer.cs](https://github.com/dshe/InternalContainer.cs) A simple IoC container in a single C# 6.0 portable class library (PCL) source file.

[Portable WebDAV Library](https://github.com/DecaTec/Portable-WebDAV-Library) Portable WebDAV Library is a fully RFC 4918 compliant WebDAV client library which is implemented das portable class library (PCL) for use on desktop environments as well as mobile devices. https://decatec.de

[Websockets.PCL](https://github.com/NVentimiglia/Websockets.PCL) C# Websockets for all platforms using native bridges

[sockets-for-pcl](https://github.com/rdavisau/sockets-for-pcl) Cross-platform socket API for Xamarin iOS/Android/Forms, Xamarin.Mac/MonoMac, Windows Phone 8/8.1, Windows Store and Windows Desktop.

[Polly](https://github.com/App-vNext/Polly) Polly is a .NET 3.5 / 4.0 / 4.5 / PCL library that allows developers to express transient exception handling policies such as Retry, Retry Forever, Wait and Retry or Circuit Breaker in a fluent manner.



[PCLCrypto](https://github.com/AArnott/PCLCrypto) PCLCrypto is an open source library that provides portable class library authors with cryptographic APIs that invoke platform-specific crypto automatically.

[BouncyCastle-PCL](https://github.com/onovotny/BouncyCastle-PCL) PCL Version of BouncyCastle targetting .NET, SL, WP, WinRT, .NET Core and CoreCLR. The Bouncy Castle Crypto package is a C# implementation of cryptographic algorithms and protocols, it was developed by the Legion of the Bouncy Castle, a registered Australian Charity, with a little help! The Legion, and the latest goings on with this package, can be found at http://www.bouncycastle.org. In addition to providing basic cryptography algorithms, the package also provides support for CMS, TSP, X.509 certificate generation and a variety of other standards such as OpenPGP.

[BCLExtensions](https://github.com/csMACnz/BCLExtensions) Base Class Library Extensions for C# base class library classes, across .Net, Silverlight, WinRT. You can view the list if extensions available and future extensions to come on the [Extensions Wiki Page](https://github.com/csMACnz/BCLExtensions/wiki/Extensions).

[ExcelReader-WinRT](https://github.com/BananaScheriff/ExcelReader-WinRT) Excel sheets reader for Uniwersal Windows Platform

[ValidatableBase](https://github.com/scionwest/ValidatableBase) Model Validation for Universal WinRT Apps through delegate method invocation per-property or DataAnnotation styled attribute validation. Added validation interception support. You may now have the built-in validation rules invoke a delegate method. This provides you with a little more flexibility when performing validation. You may piggy back on top of existing rules for minor checks instead of resorting to a full delegate validation method. By letting your model inherit from ValidatableBase, you can force validation checks on a model from within your view model. Binding to the view is really easy, using one of the two provided converters. The library comes with support for validating minimum and maximum numeric values, ranges of numeric values, string length, null objects, empty collections, empty or null strings and custom delegate method invocation. If you want to write your own attribute validation, you just need to implement IValidationRule and then decorate your object.

[Yort.Ntp](https://github.com/Yortw/Yort.Ntp) A cross platform NTP client library for .Net platforms. Allows you to easily retrieve an accurate, current date & time from internet NTP servers. For platforms that support task based async: var client = new Yort.Ntp.NtpClient(); var currentTime = await client.RequestTimeAsync();

[Yort.Http.ClientPipeline](https://github.com/Yortw/Yort.Http.ClientPipeline) A collection of handlers, filters, extensions and other stuff related to System.Net.Http.HttpClient and Windows.Web.Http.HttpClient.

[Really Simple Service Discovery Protocol](https://github.com/Yortw/RSSDP) RSSDP is a 100% .Net implementation of the Simple Service Discovery (SSDP) protocol that is part of the Universal Plug and Play (UPnP) standard. SSDP allows you to discover devices and services on a (local) network. RSSDP is designed primarily to publish and discover custom or 'basic' devices, and as such does not implement the full UPnP device architecture. If you are looking to build a device for which a full UPnP device schema exists, this is not the library for you (sorry! though I guess you can fork and extend if you like). If you are looking for a way to discover a custom service (such as a proprietary REST or SOAP service) from a device, RSSDP might be the solution for you.

[PoolSharp](https://github.com/Yortw/PoolSharp) PoolSharp is a simple, light weight, thread safe object pool. It also supports pooling of disposable types, managing the life time of pooled objects and performing early dispose when possible. Pool implementations implement a simple common interface, so they can be mocked or replaced with alternatives.

[UniversalClassLibrary](https://github.com/Meowtrix/UniversalClassLibrary) Class library for all .NET platforms. (Guessing that Universal actually includes Universal Windows Platform)

# Media
[MediaFoundation](https://github.com/AndrewGaspar/MediaFoundation) Some helper functions for WinRT for getting media information about some URL

[FFMPEGHelper](https://github.com/krishnan-unni/FFMPEGHelper) Windows 10 Universal WinRT component for FFMPEG library

[Universal.WebP](https://github.com/FrayxRulez/Universal.WebP) This repository contains a Windows Runtime Component that wraps up libwebp and allows to decode static and animated WEBP images.

[BreadPlayer](https://github.com/theweavrs/BreadPlayer) Bread Player is a music player with tons of features coded in CSharp/.NET Core for the Universal Windows 10 Platform (UWP). This project is being developed to acknowledge and rectify the scarcity of Music players in Windows 10 Store and also to provide flawless and feature-rich Music player to the end-user. It is still in a very experimental stage so much so that not even the UI is ready at the moment. [Roadmap](https://github.com/theweavrs/BreadPlayer/wiki/Roadmap)

[Microsoft Media Platform's Player Framework](http://playerframework.codeplex.com/) An open source, robust video player framework for Windows 10, Windows 8, HTML5, Silverlight, Windows Phone and other application platforms. 

![](http://download-codeplex.sec.s-msft.com/Download?ProjectName=playerframework&DownloadId=527525)

Video players can be incredibly difficult to build. When developers require support for adaptive streaming, closed captioning, advertising standards integration, DVR-style playback control, and other advanced features, the complexity of their video player grows exponentially. Over the last few years at Microsoft we have helped build some of the most advanced video applications on the Web including the browser-based experience for the Beijing and Vancouver Olympics with NBC Sports, the last three seasons of NBC's Sunday Night Football (including the 2012 Super Bowl), the CBS March Madness college basketball tournament, Wimbledon, and a number of other major, live events with millions of simultaneous users. As a part of those projects we have developed one of the most powerful video players on the planet. And we've decided to share it with everyone, for free.  The Microsoft Media Platform's Player Framework is an open source video player that we continue to develop and evolve. It is available for Silverlight, HTML5, Windows Phone, Xbox, and now, in our latest release, Windows 10 UWP applications. And it's fully open source!


# Graphics 2D
[Win2D](https://github.com/Microsoft/Win2D) Win2D is an easy-to-use Windows Runtime API for immediate mode 2D graphics rendering with GPU acceleration. It is available to C# and C++ developers writing Windows apps for Windows 8.1, Windows Phone 8.1 and Windows 10. It utilizes the power of Direct2D, and integrates seamlessly with XAML and CoreWindow. http://microsoft.github.io/Win2D (https://github.com/Microsoft/Win2D-Samples)

[SvgForXaml](https://github.com/mntone/SvgForXaml) Draw image from svg file with Win2D

[XamlAnimatedGif](https://github.com/XamlAnimatedGif/XamlAnimatedGif) A simple library to display animated GIF images in XAML apps (WPF, WinRT, Windows Phone)

[GifImageSource](https://github.com/sskodje/GifImageSource) GifImageSource is a Windows Runtime Component for WinRT projects, made for rendering GIF images in a resource efficient way using Direct2D.


[WriteableBitmapEx](https://github.com/teichgraf/WriteableBitmapEx) The WriteableBitmapEx library is a collection of extension methods for the WriteableBitmap. The WriteableBitmap class is available for all XAML flavors including Windows Phone, WPF, WinRT Windows Store XAML, (Windows 10) UWP and Silverlight. It was even ported to Windows Embedded. WriteableBitmapEx allows the direct manipulation of a bitmap and can be used for image manipulation, to generate fast procedural images by drawing directly to a bitmap and more. The WriteableBitmap API is very minimalistic and there's only the raw Pixels array for such operations. The WriteableBitmapEx library tries to compensate that with extensions methods that are easy to use like built in methods and offer GDI+ like functionality. The library extends the WriteableBitmap class with elementary and fast (2D drawing) functionality, conversion methods and functions to combine (blit) WriteableBitmaps. The extension methods are grouped into different C# files using a partial class approach. It is possible to include just a few methods by using the specific source code files directly or the full functionality via the built binaries. 

[ImagingUWP](https://github.com/asiertarancon/ImagingUWP) UWP app with Lumia Imaging SDK

# Graphics 3D
[SharpDX](http://sharpdx.org/) SharpDX is an open-source managed .NET wrapper of the DirectX API. Windows Store Apps PCL .NET 4.6+ including the Universal Windows Platform (UWP) & Windows Desktops that supports .NET 4.5+
https://github.com/sharpdx/SharpDX 

[SharpDX Samples](https://github.com/sharpdx/SharpDX-Samples) This repository contains more than 100+ code samples using SharpDX

[SharpDXTex](https://github.com/oguna/SharpDXTex) Texture library for SharpDX3.0 - Managed wrapper of DirectXTex - In SharpDX3.0, D3DX libraries, Texture.LoadFromFile or Texture.LoadFromStream, were removed. If you want to use taht functions, you can use this library alternatively.

[SharpDXTutorials](https://github.com/mrjfalk/SharpDXTutorials) Code for my SharpDX Tutorials at www.johanfalk.eu.

[SharpDX D3D12 Hello World](https://github.com/RobyDX/SharpDX_D3D12HelloWorld)  DirectX12 Hello World samples created with SharpDx and C# http://www.notjustcode.it - This sample are porting of original D3D12 Hello World realised by Microsoft. I've converted this samples in C# using last version of SharpDx and [DirectX11 Tutorial](https://github.com/RobyDX/SharpDX_Demo) This is a collection of demos that show how to use DirectX11 tecnology with SharpDX library (http://sharpdx.org/) and C# in .Net 4.5 platform Every source want to be as easy as possible to give attention to the arguments of each one.


[DirectCompositionDirectX12Sample](https://github.com/PJayB/DirectCompositionDirectX12Sample) A demonstration of DirectComposition and DirectX 12 interoperability - This sample demonstrates how to implement DirectComposition alongside DirectX 12. DirectComposition allows you to efficiently composite your rendered scene onto other windows using hardware acceleration.  For more information, see:
- [MSDN page for DirectComposition](https://msdn.microsoft.com/en-us/library/windows/desktop/hh437371(v=vs.85).aspx)
- [Tutorial](http://blog.pjblewis.com/efficient-alpha-blended-windows-directcomposition/)
- This sample is based on Microsoft's [D3D12HelloTexture sample](https://github.com/Microsoft/DirectX-Graphics-Samples). 

[SDL2](https://libsdl.org/) "Simple DirectMedia Layer is a cross-platform development library designed to provide low level access to audio, keyboard, mouse, joystick, and graphics hardware via OpenGL and Direct3D." There is suppossed to be a UWP port of SDL somewhere at https://libsdl.org/ but I haven't found it. I was also given this link: https://github.com/emscripten-ports/SDL2 - At the moment there is no feeback on how robust this support is and how well in interacts with Windows Composition etc. 

[DirectXTK12](https://github.com/Microsoft/DirectXTK12) The DirectX Tool Kit (aka DirectXTK12) is a collection of helper classes for writing DirectX 12 code in C++ https://blogs.msdn.microsoft.com/chuckw/2016/07/18/directx-tool-kit-for-directx-12/

[DirectXTK](https://github.com/Microsoft/DirectXTK) The DirectX Tool Kit (aka DirectXTK) is a collection of helper classes for writing DirectX 11.x code in C++ http://blogs.msdn.com/b/chuckw/archive/2012/03/02/directxtk.aspx

[DirectXMath](https://github.com/Microsoft/DirectXMath) DirectXMath is an all inline SIMD C++ linear algebra library for use in games and graphics apps https://blogs.msdn.microsoft.com/chuckw/2012/03/26/introducing-directxmath/

[UVAtlas](https://github.com/Microsoft/UVAtlas) UVAtlas isochart texture atlas http://blogs.msdn.com/b/chuckw/archive/2014/11/14/uvatlas-return-of-the-isochart.aspx

[DirectXTex](https://github.com/Microsoft/DirectXTex) DirectXTex texture processing library http://blogs.msdn.com/b/chuckw/archive/2011/10/28/directxtex.aspx

[DirectX-Graphics-Samples](https://github.com/Microsoft/DirectX-Graphics-Samples) This repo contains the DirectX Graphics samples that demonstrate how to build graphics intensive applications on Windows.

[DXUT](https://github.com/Microsoft/DXUT) DXUT is a "GLUT"-like framework for Direct3D 11.x Win32 desktop applications; primarily samples, demos, and prototypes. http://blogs.msdn.com/b/chuckw/archive/2013/09/16/dxut-for-win32-desktop-update.aspx

[FX11](https://github.com/Microsoft/FX11) Effects for Direct3D 11 (FX11) is a management runtime for authoring HLSL shaders, render state, and runtime variables together. http://blogs.msdn.com/b/chuckw/archive/2012/10/23/effects-for-direct3d-11-update.aspx


[UVAtlas](https://github.com/Microsoft/UVAtlas) UVAtlas isochart texture atlas http://blogs.msdn.com/b/chuckw/archive/2014/11/14/uvatlas-return-of-the-isochart.aspx

[DirectXMesh](https://github.com/Microsoft/DirectXMesh) DirectXMesh geometry processing library http://blogs.msdn.com/b/chuckw/archive/2014/06/27/directxmesh.aspx performing various geometry
content processing operations including generating normals and tangent frames, triangle
adjacency computations, and vertex cache optimization.

# Game Dev

[MonoGame](https://github.com/mono/MonoGame) One framework for creating powerful cross-platform games. http://www.monogame.net MonoGame is an open source implementation of the Microsoft XNA 4.x Framework. Our goal is to make it easy for XNA developers to create cross-platform games with extremely high code reuse.

[MonoGame.Extended](https://github.com/craftworkgames/MonoGame.Extended) MonoGame.Extended is a portable class library designed to build on top of MonoGame. It may work also with XNA/FNA (not confirmed) and it should work on other platforms like Xamarin Android or iOS. If you do use it on another platform please let us know!

[FarseerPhysics.Portable](https://github.com/craftworkgames/FarseerPhysics.Portable) This is a fork of the Farseer Physics Engine found on codeplex with a few minor changes to make it work as a Portable Class Library (PCL) with the PCL version of MonoGame.

[Xenko Game Engine](https://github.com/SiliconStudio/xenko) Xenko is a powerful cross-platform game engine. Enjoy the latest features of .NET 4.6 and C#6 to write stunning games efficiently! Import your assets and build your world using the Game Studio. Create scripts with Microsoft Visual Studio and bring your game to life! Xenko is available for free using a dual license system and its source code is available on GitHub. [Xenko.com](http://xenko.com/) - [Xenko Samples](https://github.com/SiliconStudio/xenko-samples) - [Features](http://xenko.com/features/) -  [Platforms](http://xenko.com/features/platforms/)

[Unity](https://unity3d.com/)  - [Get Unity](https://unity3d.com/get-unity) -  [Platforms](https://unity3d.com/unity/multiplatform) Also supports Microsoft Hololens.

# Language

[The Visual F# compiler and tools](https://github.com/Microsoft/visualfsharp) F# is a mature, open source, cross-platform, functional-first programming language which empowers users and organizations to tackle complex computing problems with simple, maintainable, and robust code. F# is used in a wide range of application areas and is supported by Microsoft and other industry-leading companies providing professional tools, and by an active open community. You can find out more about F# at http://fsharp.org.

# Testing

Opinionated Note: There is a lot of scaffolding issues to consider for testing UWP apps and I have a healthy sckepticism of social memes such as "Agile" and "Unit Testing" so this category is essential at the bottom of my attention list so, please let me know if I have missed any libraries and tools associated with UWP Testing

[myweather](https://github.com/fernandoescolar/myweather) This is a demo of unit testing in UWP. It contains a T4 template to generate all the Spies, Stubs and Mocks of all the interfdaces found in your solution.

[xUnit.net](https://github.com/xunit/xunit) xUnit.net is a free, open source, community-focused unit testing tool for the .NET Framework. Written by the original inventor of NUnit v2, xUnit.net is the latest technology for unit testing C#, F#, VB.NET and other .NET languages. xUnit.net works with ReSharper, CodeRush, TestDriven.NET and Xamarin. It is part of the ASP.NET Open Source Gallery under the Outercurve Foundation, licensed under Apache 2 (an OSI approved license). [Getting Started with xUnit.net (Universal Windows Apps)](http://xunit.github.io/docs/getting-started-uwp.html)

[xunit-performance](https://github.com/Microsoft/xunit-performance) Provides extensions over xUnit to author performance tests.

[PCLMock](https://github.com/kentcb/PCLMock) PCLMock is a simple mocking framework in a Portable Class Library. Existing mocking frameworks, such as Moq, do not work on platforms running a limited subset of the .NET framework. Writing mocks without the aid of a framework is laborious, error-prone, and results in inconsistent code. PCLMock aims to reduce this pain.

[FluentAssertions](https://github.com/dennisdoomen/FluentAssertions) Fluent Assertions is a set of .NET extension methods that allow you to more naturally specify the expected outcome of a TDD or BDD-style test. We currently use it in all our internal and client projects, and it is used in many open-source projects. It runs on .NET 4.0, 4.5, 4.6, CoreClr, .NET Native, Windows 8.1, Silverlight 5, Windows Phone 8.0… http://www.fluentassertions.com

[FluentAssertionsEx](https://github.com/hivepeople/FluentAssertionsEx) Extensions for FluentAssertions.

[FluentAssertions.Autofac](https://github.com/awesome-inc/FluentAssertions.Autofac) Fluent Assertions extensions for Autofac

[Shouldly](https://github.com/shouldly/shouldly) Should testing for .net - the way Asserting *Should* be! http://shouldly.readthedocs.org/en/latest




# Samples for Reference or Learning


[Windows-universal-samples](https://github.com/Microsoft/Windows-universal-samples) Official API samples for the Universal Windows Platform.

[HealthClinic.biz](https://github.com/Microsoft/HealthClinic.biz) The samples contained in this repo are used to present an end-to-end demo scenario based on a fictitious B2B and multitenant system, named “HealthClinic.biz” that provides different websites, mobile apps, desktop apps, wearable apps, and services running on the latest Microsoft and open technologies aligned with announcements to showcase during … http://aka.ms/Connect

[UWPQuickStart](https://github.com/Microsoft/UWPQuickStart) Building a Universal Windows app in Visual Studio is quick and easy. We've provided a sample app that you can download and learn how the various pieces fit together. We even encourage you to customize and send a version of this app to the Windows Store!

[Windows-appsample-quizgame](https://github.com/Microsoft/Windows-appsample-quizgame) A peer-to-peer trivia game sample for the Universal Windows Platform (UWP). 

[UWP-Samples](https://github.com/Myfreedom614/UWP-Samples) Samples for Windows 10 Universal Platform

[UWP Custom Control Example](https://github.com/almirvuk/UWPCustomControlExample) In this tutorial I will demonstrate how to make your own custom control for Universal Windows Platform application. This is very handy way of making your app more modular and responsive. For this tutorial I will make "Speaker" control, for some of our conference or event App. 

[InkToolbar and Custom Dry Ink](https://github.com/mscherotter/InkToolbarAndCustomDryInk) Windows UWP Sample that demonstrate how to use the InkToolbar Control with a custom Dry Ink CanvasControl

    Implementing custom dry mode for ink
    Drawing ink using Win2D and effects
    Implementing ink erasing with the InkToolbar control with custom dry Ink
    Adding a custom button to the InkToolbar
    Rendering Win2D to be used in a Share contract
    Simultaneous pen and touch with the ScrollViewer control


# Samples That Don't Hurt Your Eyeballs

There are lots of UWP App samples but most of them look like crap either because they are meant to demo a Windows 10 UWP feature or else total lack of aesetic sense. This section will give you some hope that one day the Windows Store won't be full of junk.

This is an important category so I will really appreciate suggestions by anyone including the authors for any UWP Apps that I can add to this sub-list.

[Kliva](https://github.com/AppCreativity/Kliva) "Thanks to Kliva, you'll now be able to get a detailed overview of all your sport endevaours and the data that goes with it." - Featured at Build 2016 in session:  ["Creating Beautiful UX in a Real-World App with Visuals, Animations and Effects"](https://channel9.msdn.com/Events/Build/2016/B818) with this branch of the code: https://github.com/AppCreativity/Kliva/tree/alcatraz

[Baconit](https://github.com/QuinnDamerell/Baconit) A beatiful, powerful, reddit client for Windows 10. https://www.reddit.com/r/BaconitDev/ The highest rated reddit client for Windows Phone has been rewritten from the ground up and is now available for all Windows 10 devices. Now with a dynamic new UI, faster speeds, and features you have been asking for. Welcome to the new Baconit. We know you’re going to love it.
![](https://github.com/QuinnDamerell/Baconit/raw/develop/Media/GitHubReadme/Desktop1.png)

[MyerSplash](https://github.com/JuniperPhoton/MyerSplash) Claims to be "the best looking Wallpaper App" [here](http://juniperphoton.net/myersplash/) so let me know if you agree. An UWP app that allows you to browse and download high-quality wallpaper from Unsplash.com. To compile the project, please include [JP.Utils.UWP](https://github.com/JuniperPhoton/JP.Utils.UWP) which is the lib I am developing to the solution. 

# Samples That Don't Know They are Samples

### Any UWP App on GitHub

These are essentially samples of something or other that could be illuminating, since any OSS is there to be studied like an open book.

I will try to list anything I come across. (Just in case is isn't obvious, there are hundreds of UWP apps on GitHub, so in theory there will eventually be hundreds listed in this section since for the most part my curation is limited to not listing empty or obviously out of date projects. If it gets to that, I will make a separate page. For now, the list is short because my priority is Data, Graphics and UI projects and the selection here is just random chance.

[MultiTimer](https://github.com/KvnSmith212/MultiTimer) UWP timer app that allows for creation of many timers.

[Flavordex Tasting Journal](https://github.com/ultramega/flavordex-uwp) Flavordex Tasting Journal for The Universal Windows Platform http://flavordex.com/ [Windows Store](https://www.microsoft.com/store/apps/9nblggh5rhrx)

[CameraUWP](https://github.com/javieresc97/CameraUWP) Uwp app that uses emotion API

[MasterPasswordUWP](https://github.com/papricasix/MasterPasswordUWP) Tool for managing stateless passwords for Windows (UWP). Based on: https://github.com/Lyndir/MasterPassword (Master Password is an algorithm and Java/iOS application to solve the real trouble with passwords.http://masterpasswordapp.com/)

[UWPCMS](https://github.com/sunilmusinada/UWPCMS) no description


[FaceBattleUWP](https://github.com/JuniperPhoton/FaceBattleUWP) FaceBattle app for Universal Windows Platfrom.

[UWP Battery Tester](https://github.com/ugur2323/UWP-Battery-Tester)

[WeatherOrNot](https://github.com/TracyDa/WeatherOrNot) UWP weather app

[VideoCapture Universal App](https://github.com/pre10der89/VideoCapture) VideoCapture Universal App for Windows 8.1 and Windows UWP

[pegelalarm-uwp](https://github.com/hoenic07/pegelalarm-uwp) The Pegelalarm app for Windows 10. When the project reaches a "beta" state it will also reach the Windows Store. You can find more information about the Pegelalarm project here: http://pegelalarm.at/

[WeatherApplication](https://github.com/HeinPauwelyn/WeatherApplication) UWP project with MVVM, API's and IoC

[Flantter.MilkyWay](https://github.com/cucmberium/Flantter.MilkyWay) Flantter.MilkyWay is twitter client for UWP and 3rd generation of Flantter. http://cucmber.net/flantter/

[Unigram](https://github.com/ikarago/Unigram) Unigram – An Universal take on Telegram. Made by the community, for the community.   Windows 10 (Mobile) introduced with the Universal Windows Platform a whole list of features to make your (chatting) life easier. However, the current official Telegram-app has no signs of releasing an UWP-version with these capabilities soon. That’s why we decided to build our own.

[NASA App](https://github.com/nikitakonan/NASAapp) UWP Nasa application

[Elementary](https://github.com/ultramega/elementary-uwp) Elementary is a simple Periodic Table and element reference application for The Universal Windows Platform. Videos provided by Periodic Videos (http://www.periodicvideos.com/)
-    Zoomable Periodic Table of the Elements
-    Tap an element to view some basic details
-    Easy access to Wikipedia and a YouTube video on the element
-    Free and open source

[TeamSnapV3](https://github.com/agangal/TeamSnapV3) This is a Windows 10 app for TeamSnap (www.teamsnap.com). It uses the APIs that TeamSnap provides to build an app that mirrors TeamSnap's Android and iOS apps.  This is the 3rd revision of the original app I wrote.  It doesn't have all the features yet, and is still a work in progress. Some features are waiting for APIs to be made available. Link to the app : https://www.microsoft.com/en-us/store/apps/dugout/9nblggh5k2jd 

[WA082016](https://github.com/evnik/WA082016) Playing with Windows Universal apps <Award for Most Descriptive App Name> :)

[ENRZ.UWP](https://github.com/miao17game/ENRZ.UWP) App For ENRZ by Wallace

[DQD-UWP](https://github.com/miao17game/DQD-UWP) Dongqiudi UWP by Pao

[HomeBudgetViewer](https://github.com/lsielewicz/HomeBudgetViewer) Simple UWP app that allows to manage users expenses and icomes.

[MathExpression](https://github.com/OpportunityLiu/MathExpression) Parse math expressions, generate lambda expressions and compiled functions. For UWP.

[MatrixJar](https://github.com/Worldbeater/MatrixJar) Matrix calculator for Universal Windows 10 platform! https://www.microsoft.com/en-us/store/p/matrixjar/9nblggh530bd 
![](https://camo.githubusercontent.com/6d35073df2d56ab8b598496c702aff686648b47c/68747470733a2f2f776f726c646265617465722e6769746875622e696f2f6d6f636b7570732f4d61747269784a61722e6a7067)
MatrixJar is a matrix calculator for Universal Windows 10 platform! It can count matrices sum, multiplication, can transpose or inverse matrices or get their determinants.


[MALClient](https://github.com/Drutol/MALClient) Small client app for Myanimelist.net and Hummingbird.me - Windows 10 UWP.

[myFeed](https://github.com/Worldbeater/myFeed)  RSS reader for Universal Windows 10 platform! https://www.microsoft.com/en-us/store/apps/myfeed/9nblggh4nw02
![](https://camo.githubusercontent.com/4245d02dbdaadf86ac7f7c526573aa1b7fc84cd0/68747470733a2f2f776f726c646265617465722e6769746875622e696f2f6d6f636b7570732f6d79466565642e6a7067)
myFeed is an RSS reader for UWP platform written in C#. It can grab news from websites and save them on your device. 

[Tramline-5](https://github.com/betrakiss/Tramline-5) Universal Windows app for the Public Transport in Sofia (Bulgaria).

[OwncloudUniversal](https://github.com/pestotoast/OwncloudUniversal) Owncloud-Client for Windows Phones (Win10Mobile) or PCs

[DoubanGroup.UWP](https://github.com/scheshan/DoubanGroup.UWP) no desc - 30 stars


# Blogs and Websites convert to Apps

[Noodles-Blog-UWP](https://github.com/miao17game/Noodles-Blog-UWP) a UWP app of my Blog - Blog website: http://noodlesblog.azurewebsites.net



# Games

[Orchi's Isle, The Adventure Begins](https://github.com/orchidwarestudios/orchis-isle-uwp) Whimsical, exciting adventure game for Windows 10 devices. This project creates a 2D video game for the Universal Windows Platform (UWP). It can be played on a Windows 10 PC/Tablet. The code is written using DirectX 11, C++, and XAML. The code is currently compatible with Windows 10 desktop, tablet devices, and the XBox One console. It will not be optimized for Windows 10 phone devices.

[DotaTournamentHub](https://github.com/davidmikh/DotaTournamentHub) A UWP app that displays information about Dota 2 Tournaments & Leagues

[ToddlerBox](https://github.com/ibebbs/ToddlerBox) A UWP app for the XBox One providing visual and tactile entertainment for babies and toddlers.






# End of the List

If you have made it to the end of the list, here we have the weird and the wonderful and the questionables, just like the old maps for mariners that showed Sea Monsters at the Ends of the Earth

# Interfacing with Plants

[PlantSensor](https://github.com/ms-iot/PlantSensor) digiPlant is a Universal Windows Platform app that helps users monitor their plant. The app collects and displays tempoerature, brightness, and soil moisture data from various sensors. It runs on a Raspberry Pi and Windows 10 IoT Core. The Twitter page is currently a work in progress.

[PlantSitter](https://github.com/JuniperPhoton/PlantSitter) An UWP app that can monitor your plant's growing status in real time and provide you some advice. http://juniperphoton.net/plantsitter


# Pokemon on UWP

[PoGo](https://github.com/PoGo-Devs/PoGo) UWP Client for Pokemon Go http://www.pogo-uwp.tk

[PoGo-3D-Assets](https://github.com/PoGo-Devs/PoGo-3D-Assets) 3D-Pokemon Models for PoGo-UWP-If you want to help check out the issues and make a coment on what you are working.

[PoGo-UWP](https://github.com/ST-Apps/PoGo-UWP) PoGo for Windows 10 You can find the installation file for PoGo in Releases. Please read the whole release information before installing.[wiki](https://github.com/ST-Apps/PoGo-UWP/wiki/Home-(EN))

[PokemonGoStat](https://github.com/thegamenicorus/PokemonGoStat) C# class library used to calculate Pokemon Stats in Pokemon Go game

[PokemonGoChina](https://github.com/Afanyiyu/PokemonGoChina) This is China customised version of Pokemon Go UWP. It using the Windows anniversary SDK (10.0.14393). 

[UWP Pokedex](https://github.com/CuriousCurmudgeon/uwp_pokedex) Simple UWP pokedex app for my Intro to UWP talk at Richmond Tech

[TU6](https://github.com/pogodevorg/TU6) For the curious, this effort appears to be the origin of 3rd party Pokemon Go interfacing. "A repository to show what was done and achieved over a 3.5 day sleepless community hackathon"

[PokemonGoMap](https://github.com/tommyinb/PokemonGoMap) A C# map project

[PokemonGo-Map](https://github.com/PokemonGoMap/PokemonGo-Map) For the curious, this is Python, but surely you need to know if any dangerous Pokemons are lurking about in your neighborhood! -> Live visualization of all the pokemon in your area... and more!

![](https://camo.githubusercontent.com/61d585e7706d136694f50ed2a092661b203a0a5d/687474703a2f2f70676d2e72656164746865646f63732e696f2f656e2f6c61746573742f5f696d616765732f636f7665722e706e67)









