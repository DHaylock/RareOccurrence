#Rare Occurrence
###

##Table Creation
####Logins
```
CREATE TABLE IF NOT EXISTS `logins` (
  `id` int(10) NOT NULL AUTO_INCREMENT,
  `uniqueid` varchar(50) NOT NULL,
  `username` varchar(255) NOT NULL,
  `password` varchar(255) NOT NULL,
  `routeb` tinyint(1) NOT NULL,
  `infrequency` tinyint(1) NOT NULL,
  PRIMARY KEY (`id`)
) ENGINE=MyISAM DEFAULT CHARSET=latin1 AUTO_INCREMENT=1 ;
```

####Infrequency
```
CREATE TABLE IF NOT EXISTS `infrequency` (
  `id` int(10) NOT NULL AUTO_INCREMENT,
  `searchterm` varchar(255) NOT NULL,
  `customerid` varchar(255) NOT NULL,
  PRIMARY KEY (`id`)
) ENGINE=MyISAM DEFAULT CHARSET=latin1 AUTO_INCREMENT=1 ;
```

####RouteB
```
CREATE TABLE IF NOT EXISTS `routeb` (
  `id` int(10) NOT NULL AUTO_INCREMENT,
  `customerid` varchar(255) NOT NULL,
  `startlat` varchar(50) NOT NULL,
  `startlng` varchar(50) NOT NULL,
  `endlat` varchar(50) NOT NULL,
  `endlng` varchar(50) NOT NULL,
  `mode` varchar(50) NOT NULL,
  `optimism` varchar(50) NOT NULL,
  PRIMARY KEY (`id`),
  UNIQUE KEY `customerid` (`customerid`)
) ENGINE=MyISAM DEFAULT CHARSET=latin1 AUTO_INCREMENT=1 ;
```

##Insert Queries


##Select Queries
