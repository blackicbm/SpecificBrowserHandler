# SpecificBrowserHandler
Register the specific protocol to help the special URL to be opened in the specific browser.

You should have ever encountered such situation: There are many web systems which still need end user to open it with MS Internet Explorer, or it would not work at all. It would be annoying to copy the URL and paste it in MS Internet Explorer every time. We can find the alternatives:
- The extension like "IE Tab" to relieve this pain, but this kind of tool might not work always.
- A browser chooser, like Choosy (Mac) or BrowserChooser2 (Windows); However, it would require you to configure the preference on every PC you would use.

The way we adopt here is to register a protocol handler which will launch the specific browser directly, and also feed it the URL you are going to visit.
To treat these special URL, we might register a specific protocol handler "msie:", and we could add the prefix "msie:" to "the specified URL. When you click on these URL, e.g. msie:http://xxx.com or msie:https://xxx.com, they will be opened by MS Internet Explorer directly.