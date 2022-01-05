![Screenshot_4](https://user-images.githubusercontent.com/67419505/148230474-265a65d0-fbec-41d6-9ebd-339b38569b47.png)

**Description**
> WaveVehiclesPreview is an amazing FiveM STANDALONE resource, allowing you to exhibit your most beautiful vehicles at the dealership and offer a catalog worthy of the name!
> Every features is configurable and can be adapted to all your tastes! 

**Showcase**

![Screenshot_5](https://user-images.githubusercontent.com/67419505/148230523-7ea85b1a-125f-4bb4-9e7c-d3777944317f.png)

> Watch the [Showcase](https://www.youtube.com/watch?v=ADwWLSPWYVA) !

**Discord**
> https://discord.gg/5x2kXXkZTR

**Tebex**
> [WaveResources | Home (tebex.io)](https://waveresources.tebex.io/category/resources) - 20€ + taxes

**Features**
* resmon : 0.0ms Closed, 0.2ms opened
* Catalog
  * You can add infinite numbers of vehicles & categories in the catalogs ( like add-on/donators vehicles )
  * You can test the car during a limited time
  * Display Prices & Vehicle Statistics
  * Ability to customize vehicle
  * Ability to change vehicle colors
  * Ability to honk the horn
  * Great Camera
  * Configurable Coords & Camera
 * Exhibition
  * Authorized players can add,edit, or delete exhibitions
  * Exhibition Options
    * Vehicle spawn name
    * Vehicle position & heading according to where your gameplay camera point
    * Ability to full custom the vehicle
    * Ability to change the vehicle colors
    * Ability to rotate vehicle
    * Ability to enable drive test
* Customizable Blips & Markers
* Openable with a command that require the player to be whitelisted or have  the required job
* Anti-Glitchs
* Nice sounds
* Nices Notifications
* built-in RageUI edited
* Multiples Languages supported
* Standalone
* And more...

**Config Example**
```
waveVehiclesPreview = {
    frameWork = 'ESX', -- ESX  / QBCORE  ||| VRP not supported yet
    getSharedObject = "esx:getSharedObject", --may be QBCore:GetObject too
    Language = "EN", --FR/EN/DE/ES
    Currency = "$",
    Exhib = {
        enable = true, --require ESX , otherwise whitelist player license
        WhitelistedLicenses = {
            ["license:171a23d246444c95bd897754beb26aa197ab3570"] = true,
        },
        enableJob = true,
        requiredJob = "cardealer",
        commandName = "catalog",
        maxExhibitedVehicles = 1,
    },
    Blips = {
        enable = true,
        Sprite = 225,
        Color = 2,
        Scale = 0.7,
    },
    Markers = {
        markerDistance = 25.0,
        notificationDistance = 5.0,
        menuDrawDistanceFromMarker = 5.0,
    },

    Catalog = {
        enable = true,
        coords =  vector3(-41.21,-1081.88,26.6),
        vehicleSpawn = {coords = vector3(-15.86,-1102.76,26.67), heading = 160.0},
        driveTestSpawn = {coords = vector3(1198.631,330.31,81.99), heading = 145.0},
        driveTestSpawnFullCustom = true,
        driveTestTime = 60, -- in seconds, how many time player can drive the vehicle
        camOffset = vector3(3.0,5.0,3.0),
        vehicles = {
            ["Compacts"] = {
                {model = "blista",price = 1000 },
                {model = "dilettante",price = 1000 },
                {model = "issi2",price = 1000 },
                {model = "issi3",price = 1000 },
                {model = "panto",price = 1000 },
                {model = "prairie",price = 1000 },
                {model = "rhapsody",price = 1000 },
            },
            ["Coupes"] = {
                {model = "cogcabrio",price = 1000 },
                {model = "exemplar",price = 1000 },
                {model = "f620",price = 1000 },
                {model = "felon",price = 1000 },
                {model = "felon2",price = 1000 },
                {model = "jackal",price = 1000 },
                {model = "oracle",price = 1000 },
                {model = "oracle2",price = 1000 },
                {model = "sentinel",price = 1000 },
                {model = "sentinel2",price = 1000 },
                {model = "windsor",price = 1000 },
                {model = "windsor2",price = 1000 },
                {model = "zion",price = 1000 },
                {model = "zion2",price = 1000 },
            },
            ["Velos"] = {
                {model = "bmx",price = 1000 },
                {model = "cruiser",price = 1000 },
                {model = "fixter",price = 1000 },
                {model = "scorcher",price = 1000 },
                {model = "tribike",price = 1000 },
                {model = "tribike2",price = 1000 },
                {model = "tribike3",price = 1000 },
        
            },
            ["Muscles"] = {
                {model = "blade",price = 1000 },
                {model = "buccaneer",price = 1000 },
                {model = "buccaneer2",price = 1000 },
                {model = "chino",price = 1000 },
                {model = "chino2",price = 1000 },
                {model = "clique",price = 1000 },
                {model = "coquette3",price = 1000 },
                {model = "deviant",price = 1000 },
                {model = "dominator",price = 1000 },
                {model = "dominator2",price = 1000 },
                {model = "dominator3",price = 1000 },
                {model = "dukes",price = 1000 },
                {model = "faction",price = 1000 },
                {model = "faction2",price = 1000 },
                {model = "faction3",price = 1000 },
                {model = "ellie",price = 1000 },
                {model = "gauntlet",price = 1000 },
                {model = "gauntlet2",price = 1000 },
                {model = "hermes",price = 1000 },
                {model = "hotknife",price = 1000 },
                {model = "hustler",price = 1000 },
                {model = "impaler",price = 1000 },
                {model = "lurcher",price = 1000 },
                {model = "moonbeam",price = 1000 },
                {model = "moonbeam2",price = 1000 },
                {model = "nightshade",price = 1000 },
                {model = "phoenix",price = 1000 },
                {model = "picador",price = 1000 },
                {model = "ratloader",price = 1000 },
                {model = "ratloader2",price = 1000 },
                {model = "ruiner",price = 1000 },
                {model = "sabregt",price = 1000 },
                {model = "slamvan",price = 1000 },
                {model = "slamvan3",price = 1000 },
                {model = "stalion",price = 1000 },
                {model = "tampa",price = 1000 },
                {model = "tulip",price = 1000 },
                {model = "vamos",price = 1000 },
                {model = "vigero",price = 1000 },
                {model = "virgo",price = 1000 },
            },
            ["Vans"] = {
                {model = "bison",price = 1000 },
                {model = "bobcatxl",price = 1000 },
                {model = "burrito3",price = 1000 },
                {model = "camper",price = 1000 },
                {model = "gburrito",price = 1000 },
                {model = "minivan",price = 1000 },
                {model = "pony",price = 1000 },
                {model = "pony2",price = 1000 },
                {model = "youga",price = 1000 },
        
            },
            ["Off Road"] = {
                {model = "bfinjection",price = 1000 },
                {model = "blazer",price = 1000 },
                {model = "blazer2",price = 1000 },
                {model = "blazer4",price = 1000 },
                {model = "bifta",price = 1000 },
                {model = "bodhi2",price = 1000 },
                {model = "brawler",price = 1000 },
                {model = "brutus",price = 1000 },
                {model = "dubsta3",price = 1000 },
                {model = "dune",price = 1000 },
                {model = "freecrawler",price = 1000 },
                {model = "kamacho",price = 1000 },
                {model = "rebel2",price = 1000 },
                {model = "riata",price = 1000 },
                {model = "sandking",price = 1000 },
                {model = "sandking2",price = 1000 },
        
            },
            ["Sports Classics"] = {
                {model = "ardent",price = 1000 },
                {model = "btype",price = 1000 },
                {model = "btype2",price = 1000 },
                {model = "btype3",price = 1000 },
                {model = "casco",price = 1000 },
                {model = "cheetah2",price = 1000 },
                {model = "coquette2",price = 1000 },
                {model = "fagaloa",price = 1000 },
                {model = "feltzer3",price = 1000 },
                {model = "gt500",price = 1000 },
                {model = "infernus2",price = 1000 },
                {model = "jb700",price = 1000 },
                {model = "mamba",price = 1000 },
                {model = "monroe",price = 1000 },
                {model = "peyote",price = 1000 },
                {model = "pigalle",price = 1000 },
                {model = "rapidgt3",price = 1000 },
                {model = "retinue",price = 1000 },
                {model = "stinger",price = 1000 },
                {model = "stingergt",price = 1000 },
                {model = "stromberg",price = 1000 },
                {model = "swinger",price = 1000 },
                {model = "torero",price = 1000 },
                {model = "tornado",price = 1000 },
                {model = "tornado2",price = 1000 },
                {model = "turismo2",price = 1000 },
                {model = "viseris",price = 1000 },
                {model = "ztype",price = 1000 },
        
            },
            ["Sports"] = {
                {model = "alpha",price = 1000 },
                {model = "banshee",price = 1000 },
                {model = "bestiagts",price = 1000 },
                {model = "blista3",price = 1000 },
                {model = "buffalo",price = 1000 },
                {model = "buffalo2",price = 1000 },
                {model = "buffalo3",price = 1000 },
                {model = "carbonizzare",price = 1000 },
                {model = "comet2",price = 1000 },
                {model = "comet3",price = 1000 },
                {model = "comet4",price = 1000 },
                {model = "comet5",price = 1000 },
                {model = "coquette",price = 1000 },
                {model = "deveste",price = 1000 },
                {model = "elegy",price = 1000 },
                {model = "elegy2",price = 1000 },
                {model = "feltzer2",price = 1000 },
                {model = "flashgt",price = 1000 },
                {model = "furoregt",price = 1000 },
                {model = "fusilade",price = 1000 },
                {model = "futo",price = 1000 },
                {model = "gb200",price = 1000 },
                {model = "hotring",price = 1000 },
                {model = "jester",price = 1000 },
                {model = "jester2",price = 1000 },
                {model = "khamelion",price = 1000 },
                {model = "kuruma",price = 1000 },
                {model = "lynx",price = 1000 },
                {model = "massacro",price = 1000 },
                {model = "massacro2",price = 1000 },
                {model = "neon",price = 1000 },
                {model = "ninef",price = 1000 },
                {model = "ninef2",price = 1000 },
                {model = "omnis",price = 1000 },
                {model = "pariah",price = 1000 },
                {model = "penumbra",price = 1000 },
                {model = "raiden",price = 1000 },
                {model = "rapidgt",price = 1000 },
                {model = "rapidgt2",price = 1000 },
                {model = "ruston",price = 1000 },
                {model = "schafter2",price = 1000 },
                {model = "schafter3",price = 1000 },
                {model = "schlagen",price = 1000 },
                {model = "schwarzer",price = 1000 },
                {model = "sentinel3",price = 1000 },
                {model = "seven70",price = 1000 },
                {model = "specter",price = 1000 },
                {model = "sultan",price = 1000 },
                {model = "surano",price = 1000 },
                {model = "tropos",price = 1000 },
                {model = "verlierer2",price = 1000 },
        
            },
            ["Berlines"] = {
                {model = "asea",price = 1000 },
                {model = "asterope",price = 1000 },
                {model = "cog55",price = 1000 },
                {model = "cognoscenti",price = 1000 },
                {model = "emperor",price = 1000 },
                {model = "fugitive",price = 1000 },
                {model = "glendale",price = 1000 },
                {model = "ingot",price = 1000 },
                {model = "intruder",price = 1000 },
                {model = "premier",price = 1000 },
                {model = "primo",price = 1000 },
                {model = "primo2",price = 1000 },
                {model = "romero",price = 1000 },
                {model = "stafford",price = 1000 },
                {model = "stanier",price = 1000 },
                {model = "surge",price = 1000 },
                {model = "superd",price = 1000 },
                {model = "tailgater",price = 1000 },
                {model = "warrener",price = 1000 },
                {model = "washington",price = 1000 },
        
            },
            ["Supers"] = {
                {model = "adder",price = 1000 },
                {model = "autarch",price = 1000 },
                {model = "banshee2",price = 1000 },
                {model = "bullet",price = 1000 },
                {model = "cheetah",price = 1000 },
                {model = "cyclone",price = 1000 },
                {model = "entity2",price = 1000 },
                {model = "fmj",price = 1000 },
                {model = "gp1",price = 1000 },
                {model = "infernus",price = 1000 },
                {model = "italigtb",price = 1000 },
                {model = "italigtb2",price = 1000 },
                {model = "nero",price = 1000 },
                {model = "nero2",price = 1000 },
                {model = "osiris",price = 1000 },
                {model = "penetrator",price = 1000 },
                {model = "pfister811",price = 1000 },
                {model = "prototipo",price = 1000 },
                {model = "reaper",price = 1000 },
                {model = "sc1",price = 1000 },
                {model = "sheava",price = 1000 },
                {model = "sultanrs",price = 1000 },
                {model = "specter2",price = 1000 },
                {model = "t20",price = 1000 },
                {model = "taipan",price = 1000 },
                {model = "tempesta",price = 1000 },
                {model = "turismor",price = 1000 },
                {model = "tyrant",price = 1000 },
                {model = "tyrus",price = 1000 },
                {model = "vacca",price = 1000 },
                {model = "vagner",price = 1000 },
                {model = "visione",price = 1000 },
                {model = "voltic",price = 1000 },
                {model = "xa21",price = 1000 },
                {model = "zentorno",price = 1000 },
        
            },
            ["SUVs"] = {
                {model = "baller",price = 1000 },
                {model = "baller2",price = 1000 },
                {model = "bjxl",price = 1000 },
                {model = "cavalcade",price = 1000 },
                {model = "everon",price = 1000 },
                {model = "contender",price = 1000 },
                {model = "dubsta",price = 1000 },
                {model = "dubsta2",price = 1000 },
                {model = "fq2",price = 1000 },
                {model = "granger",price = 1000 },
                {model = "gresley",price = 1000 },
                {model = "habanero",price = 1000 },
                {model = "huntley",price = 1000 },
                {model = "mesa",price = 1000 },
                {model = "patriot",price = 1000 },
                {model = "radi",price = 1000 },
                {model = "rocoto",price = 1000 },
                {model = "seminole",price = 1000 },
                {model = "toros",price = 1000 },
                {model = "xls",price = 1000 },
        
            },
            ["Donators"] = {
                -- yes you can add categories of your choice :)
            },
        }
    }
}
```
