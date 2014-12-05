Country sources are configured in this repository.
=======

You can add any source for any country. Simply use the two letters from [ISO 3166-1 alpha-2](http://en.wikipedia.org/wiki/ISO_3166-1_alpha-2) codes when adding a new country. Then the file containing the sources should contain the 2 letters country codes + `-sources.xml`.

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
