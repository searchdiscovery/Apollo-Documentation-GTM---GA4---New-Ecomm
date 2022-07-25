# Page Load Started

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ page_data: null });  // Clear the previous page_data object.
dataLayer.push({
  "event": "page_view",
  "detailed_event": "Page Load Started",
    "page_data": {
        "country": "<country>",
        "day_of_week": "<day_of_week>",
        "hour": "<hour>",
        "language": "<language>",
        "name": "<name>",
        "page_hash": "<page_hash>",
        "page_location": "<page_location>",
        "page_path": "<page_path>",
        "page_query_string": "<page_query_string>",
        "page_title": "<page_title>",
        "pages_viewed_num_visit": "<pages_viewed_num_visit>",
        "platform_version": "<platform_version>",
        "site_country": "<site_country>",
        "site_language": "<site_language>",
        "site_name": "<site_name>",
        "site_section": "<site_section>",
        "site_section2": "<site_section2>",
        "site_type": "<site_type>",
        "type": "<type>",
        "weekday_or_weekend": "<weekday_or_weekend>"
    },
    "user_data": {
        "user_id": "<user_id>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|page_data.country|string|The country the site is associated with.||||||||
|page_data.day_of_week|string|The day of the week the activity occured.||||||||
|page_data.hour|string|The time of activity at the top of the hour.||||||||
|page_data.language|string|The language of the current page, usually pulled from the &lt;html&gt; tag lang attribute.||||||||
|page_data.name|string|Captures the name of the page the user is on|product - XYZ123, Mens - Tops - Sweaters, Order Confirmation|||||||
|page_data.page_hash|string|Does the link point to a different domain?||||||||
|page_data.page_location|string|The url of the page currently being viewed.||||||||
|page_data.page_path|string|Captures the path portion of the page URL.||||||||
|page_data.page_query_string|string|This parameter is already configured by Google Tag Manager and Google Analytics.||||||||
|page_data.page_title|string|The title of the page currently being viewed, generally available in &lt;title&gt;.||||||||
|page_data.pages_viewed_num_visit|string|Running total of how many pages or screens a visitor had viewed at the time they took a website or mobile app action. Count re-starts with each visit.||||||||
|page_data.platform_version|string|The platform used to share content||||||||
|page_data.site_country|string|Captures the country associated with website or mobile app activity.|US, CA, FR, UK|^[A-Z]{2}$||||||
|page_data.site_language|string|Captures the language associated with website or mobile app activity.|en-us, en-gb, ch-cn, fr-ca, fr-fr, da|^[a-z]{2}([-]{1}[a-z]{2}){0,1}$||||||
|page_data.site_name|string|Common language used within the business to refer to the website. May be specific County Sites.|Prospecting-EU, Prospecting-US, Member Portal, Shop-CA, Shop-US, Shop-EU|||||||
|page_data.site_section|string|The section of the site that the current page resides in. site\_section2 through site\_section5can also be used if the site has many sections.||||||||
|page_data.site_section2|string|Captures the sub-section of the site where the page being viewed is located|Shop &gt; Kids, Shop &gt; Mens, Shop &gt; Womens|||||||
|page_data.site_type|string|Common language description of the site type of purpose. May be used to group siteName.|Prospecting, Shop, Members, Brand|||||||
|page_data.type|string|The type of page currently viewed.|home, pdp, article|||||||
|page_data.weekday_or_weekend|string|Whether it was a weekday or weekend when the activity occurred.||||||||
|user_data.user_id|string|The id of the user currently logged in to the site, if the site offers authentication and the user is authenticated.|123456, abc123|||||||




