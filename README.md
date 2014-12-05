The Geopera Job Opportunities Sources are configured in this repository.
=======

You can add any source.
The implementation should be found in crawler package. 

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
