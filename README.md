# IP2Location ES6 Module
## Install

`npm install ip2location-es6`

## Response Data

    "ip": "?",
    "ip_no": "?",
    "country_short": "?",
    "country_long": "?",
    "region": "?",
    "city": "?",
    "isp": "?",
    "latitude": "?",
    "longitude": "?",
    "domain": "?",
    "zipcode": "?",
    "timezone": "?",
    "netspeed": "?",
    "iddcode": "?",
    "areacode": "?",
    "weatherstationcode": "?",
    "weatherstationname": "?",
    "mcc": "?",
    "mnc": "?",
    "mobilebrand": "?",
    "elevation": "?",
    "usagetype": "?",
    "status": "?"
    
## Function

```javascript
IP2Location_query(my_ip, ip_type, data)
IP2Location_get_all(my_ip)
IP2Location_get_areacode(my_ip) 
IP2Location_get_city(my_ip) 
IP2Location_get_country_long(my_ip) 
IP2Location_get_country_short(my_ip) 
IP2Location_get_domain(my_ip) 
IP2Location_get_elevation(my_ip) 
IP2Location_get_iddcode(my_ip) 
IP2Location_get_isp(my_ip) 
IP2Location_get_latitude(my_ip) 
IP2Location_get_longitude(my_ip) 
IP2Location_get_mcc(my_ip) 
IP2Location_get_mnc(my_ip) 
IP2Location_get_mobilebrand(my_ip) 
IP2Location_get_netspeed(my_ip) 
IP2Location_get_region(my_ip) 
IP2Location_get_timezone(my_ip) 
IP2Location_get_usagetype(my_ip) 
IP2Location_get_weatherstationcode(my_ip) 
IP2Location_get_weatherstationname(my_ip) 
IP2Location_get_zipcode(my_ip)
```

## Usage demo

```javascript
const IP2Location = require('ip2location-es6');
let ip2loc = new IP2Location(process.env.DB_IP2LOCATION_BIN_PATH);
let result = ip2loc.IP2Location_get_all('8.8.8.8');
console.log(result);
```