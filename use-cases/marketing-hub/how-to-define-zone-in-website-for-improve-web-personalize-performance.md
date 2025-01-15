# How to define zone in website for improve web personalize performance

**Usage scenario:** Currently, when entering a web page, the CDP will return all variants that target the events invoked on this page. Therefore, for improve website personalize performance , the client can actively transmit the zone\_code according to each desired event. The CDP will only return variants that target that zone on that event.**Guidelines:**

1. 1.Completed website integration with CDP: Add main script, event script, ... **(Required).**
2. 2.Planning ad placement and creating a zone
3. 3.Add the script **"\_cdp365JourneySetting "**

### 1. Completed website integration with CDP: Add the main script, event script, ... <a href="#id-1.-completed-website-integration-with-cdp-add-the-main-script-event-script" id="id-1.-completed-website-integration-with-cdp-add-the-main-script-event-script"></a>

### 2. Planning ad placement and creating a zone <a href="#id-2.-planning-a-d-placement-and-creating-a-zone" id="id-2.-planning-a-d-placement-and-creating-a-zone"></a>

You can see a sample display location plan here: [Example - Planning zone](https://docs.google.com/spreadsheets/d/1l9eFFy-92Vppuq1la9TREXO9fz3AMgCER8JQKO_jjWg/edit#gid=0)​You can see instructions for creating zones here: [How to create a new "Ad Zone"](https://app.gitbook.com/o/-LzunofLVjpTa_-p1PQt/s/mECwNqMNUmu6OXHSYgDv/quick-start-guide/how-to-create-a-new-ad-zone)​

### 3. Add the script "\_cdp365JourneySetting" <a href="#id-3.-add-the-script-_cdp365journeysetting" id="id-3.-add-the-script-_cdp365journeysetting"></a>

Structure:

```
<script>
   var _cdp365JourneySetting = {
    jrequest_events: [{
        event_category: "EVENT_CATEGORY_NAME_CODE1",
        event_action: "EVENT_ACTION_NAME_CODE1"
    }, {
        event_category: "EVENT_CATEGORY_NAME_CODE2",
        event_action: "EVENT_ACTION_NAME_CODE2"
    }],
    jrequest_zones: ["ZONE_CODE1", "ZONE_CODE2"]
}
</script>
```

* Add the script to the "HEAD" tag on the pages where you want to specify the event and zone to display the ad
* **jrequest\_events:** list of events used to deliver advertising
  * EVENT\_CATEGOR&#x59;_\__&#x4E;AME\_CODE1, EVENT\_ACTION\_NAME\_CODE1 là code của event mà bạn dựa vào để delivery ad trên page
  * For example:

| Events           | event\_category\_name\_code | event\_action\_name\_code |
| ---------------- | --------------------------- | ------------------------- |
| **Pageview**     | **pageview**                | **view**                  |
| **View Product** | **product**                 | **view**                  |

* **jrequest\_zones:** The list of zones will display ads on the page
  * ZONE\_CODE1, ZONE\_CODE2: Zone code of Zone that you created
  * You can see how to create a zone and get the zone code [here](broken-reference)&#x20;

Code example:

```
<script>
    var _cdp365JourneySetting = {
    jrequest_events: [{
        event_category: "pageview",
        event_action: "view"
    }],
    jrequest_zones: [
          "div_asm_zone_code1"
    ]
}
</script>
```

**If you want to trigger all events for all zones, then set up a value like that**

Code example:

```
<script>
   var _cdp365JourneySetting = {
	 jrequest_events: "*",
         jrequest_zones: "*"
   }
</script>
```

**If you don't want push event delivery and do not load the media file template**

* jrequest\_zones: "none"

Code example:

```
<script>
    var _cdp365JourneySetting = {
    jrequest_events: [{
        event_category: "pageview",
        event_action: "view"
    }],
    jrequest_zones: "none"
}
</script>
```
