{
  "/" : {
    "path" : "/",
    "security" : {
      "module" : "EMBEDED",
      "config" : {
        "users" : [ {
          "username" : "admin",
          "password" : "pwd",
          "roles" : [ "admin" ]
        }, {
          "username" : "support",
          "password" : "pwd",
          "roles" : [ "support" ]
        }, {
          "username" : "user",
          "password" : "pwd"
        } ]
      },
      "classPath" : [ ]
    },
    "langFolder" : "${webswing.configDir}/lang",
    "homeDir" : "${user.dir}",
    "allowedCorsOrigins" : [ "*" ],
    "dataStore": {
        "module": "FILESYSTEM",
        "config": {
            "threadDumpsFolder": "C:/work/dataStore/threadDumps",
            "recordingsFolder": "C:/work/dataStore/recordings",
            "transferFolder": "C:/work/dataStore/transfer"
        }
    }
  },
  "/swingset3" : {
    "path" : "/swingset3",
    "name" : "SwingSet3",
    "webFolder" : "${webswing.rootDir}/apps/SwingSet3/webroot",
    "security" : {
      "module" : "INHERITED",
      "config" : null,
      "classPath" : [ ]
    },
    "icon" : "${webswing.rootDir}/apps/SwingSet3/icon.png",
    "webHomeDir" : "${webswing.rootDir}/apps/SwingSet3",
    "langFolder" : "${webswing.configDir}/lang",
    "uploadMaxSize" : 5,
    "maxClients" : 100,
    "sessionMode" : "CONTINUE_FOR_BROWSER",
    "allowStealSession" : true,
    "autoLogout" : true
  }
