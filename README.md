Geopra country sources are configured in this repository.
=======

You can add any source for any country. Simply use the ISO 3166-1 alpha-2 convention when adding a new entry. Then the file containing the sources should contain the 2 letters + sources.xml.

There are several implementation for crawlers (at the end they should just return a Job Description):
* com.geopera.crawler.impl.RssReaderWeekDay
* ...
* If it does not suite any of this feel free to write your own or simply ask us to do it.

```XML
<source-list>
	<source id="net-empregos">
		<link value="http://feeds.feedburner.com/net-empregos?format=xml"/>
		<crawler impl="com.geopera.crawler.impl.RssReaderWeekDay" />
		<img src="http://www.net-empregos.com/images/logo_net3.png" />
	</source>
	<source id="source-B">
		<link value="http://feeds.feedburner.com/net-empregos?format=xml"/>
		<crawler impl="com.geopera.crawler.impl.RssReaderWeekDay" />
		<img src="http://www.net-empregos.com/images/logo_net3.png" />
	</source>
</source-list>
```
