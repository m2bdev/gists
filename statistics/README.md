# Basetool Statistics

Paste the following script inside the body tag of each page that display a detailed basetool business presentation. You need to replace {BUSINESS_ID} with the integer id of the business and {CHANNEL_ID} with the integer id of the basetool channel.

```javascript
<!-- Stats -->
<script type="text/javascript">
    var _btstats = _btstats || {};
    _btstats.id = {BUSINESS_ID};
    _btstats.channel = {CHANNEL_ID};
    (function () {
        var btscript = document.createElement('script'); btscript.type = 'text/javascript'; btscript.async = true;
        btscript.src = ('https:' == document.location.protocol ? 'https://' : 'http://') + 'stats.basetool.se/script.js';
        var el = document.getElementsByTagName('script')[0]; el.parentNode.insertBefore(btscript, el);
    })();
</script>
```
