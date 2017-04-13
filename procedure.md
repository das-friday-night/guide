# week1: create server 
	*routering
	*generate short url: decimal to 62 base convertion

# week2: create client
	*anuglar routering
	*angular service: seperate view and http request
	*server connect mongoDB, client http GET/POST for data
		*mongoose
		*body-parser

# week3: 
	client: 
		*[ng2-charts](http://valor-software.com/ng2-charts/)

	server: 
		*[user agent](https://github.com/biggora/express-useragent)
		*[geoip-lite]
		*express middleware: rest router, redirect router

	getstats:
		at client, it is a http GET request to server
		at server, it is a aggregation (short_url -> time -> group) on MongoDB

	parseStats:
		only at server: for visit, parse its into a stats-model(a mongoDB model).
		the parse data is consists of 
			{ 
				short url, 
				ip, 
				geo location, 
				referrer in http header, 
				platform,
				browser,
				timestamp
			}




