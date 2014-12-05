Country sources are configured in this repository.
=======

Geopera is made for you and by you. Any country and any job opportunity source can be added. The convention is to use the two letters code from [ISO 3166-1 alpha-2](http://en.wikipedia.org/wiki/ISO_3166-1_alpha-2) standard when adding a new country. Then the file containing the sources should be named 2LETTERSISOCODE-`-sources.xml`.

For example, here we have `PT-sources.xml` placed under the directory `PT` (Portugal).

```XML
<source-list> 
	<source id="net-empregos"> <!-- an ID specifying the source, typically the name of the web site" -->
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
There are several implementation for crawlers (at the end they should just return a Job Description):
* com.geopera.crawler.impl.RssReaderWeekDay
* ...
* If it does not suite any of this feel free to write your own or simply ask us to do it.

