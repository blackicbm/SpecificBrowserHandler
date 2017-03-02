# SpecificBrowserHandler

## Briefing ##
Register the specific protocol to help the special URL to be opened in the specific browser.

## Introduction ##
You should have ever encountered such situation: There are many web systems which still need end user to open it with MS Internet Explorer, or it would not work at all. It would be annoying to copy the URL and paste it in MS Internet Explorer every time. We can find the alternatives:
- The extension like "IE Tab" to relieve this pain, but this kind of tool might not work always.
- A browser chooser, like [Choosy](https://www.choosyosx.com/) or [BrowserChooser2](https://bitbucket.org/gmyx/browserchooser2); However, it would require you to configure the preference on every PC you would use.

The way we adopt here is to register a protocol handler which will launch the specific browser directly, and also feed it the URL you are going to visit.
To treat these special URL, we might register a specific protocol handler "msie:", and we could add the prefix "msie:" to "the specified URL. When you click on these URL, e.g. msie:http://xxx.com or msie:https://xxx.com, they will be opened by MS Internet Explorer directly.

## Sample ##

| Original               | Changed to                  |
|------------------------|-----------------------------|
| http://www.google.com  | `msie:http://www.google.com`  |
| https://www.google.com | `msie:https://www.google.com`  |

>
Notice: this way only works for Windows system only!!


## Installation ##
>
1. Download the corresponding .reg file
2. Double click on it to execute the downloaded registry file
3. Done
