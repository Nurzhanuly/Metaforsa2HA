 - API v_2 settings: LT Setup->General->API
 - address for websocket: 192.168.1.111:2041/api, 192.168.1.111 ip of de-mg or metaforsa, 2041 default port for websocket API	 
 - communication with server have next format:
 	- 10 bytes header. first 4 bytes is length of packet, and next 6 bytes is '-JSON-'. Length of packet is length of json request + 6 bytes
 	- request in json format
 - first request after connect is:
 {
    "request": "authorize",
    "key": "1212121212121212" 
  }

  where key is special key for API, added in LT Setup->Security, Access keys, with name TCP-API(that name is required)
