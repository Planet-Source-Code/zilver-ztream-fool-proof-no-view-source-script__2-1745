<div align="center">

## Fool Proof No View Source Script


</div>

### Description

Makes it kind of hard to get the source from a page.

This code has been on javascripts.com for a while and I won code of the month ince with it, but I also recived over 11500 mails becuase of it so I hope that wont be needed here.
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Zilver Ztream](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/zilver-ztream.md)
**Level**          |Beginner
**User Rating**    |1.5 (6 globes from 4 users)
**Compatibility**  |
**Category**       |[Security](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/security__2-74.md)
**World**          |[Java](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/java.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/zilver-ztream-fool-proof-no-view-source-script__2-1745/archive/master.zip)





### Source Code

```
Add this line to/ instead of your body tag:
(In a standalone HTML file before your protected page)
<body bgcolor=black onload="window.open('fullproof.htm','','halfscreen,scrollbars')">
ADD this script at the bottom of your page, just before your </body> tag.
(in the page you want to protect)
<script language=JavaScript>
 <!--
var message="ENTER YOUR CUSTOM MESSAGE HERE";
function click(e) {
if (document.all) {
if (event.button == 2) {
alert(message);
return false;
}
}
if (document.layers) {
if (e.which == 3) {
alert(message);
return false;
}
}
}
if (document.layers) {
document.captureEvents(Event.MOUSEDOWN);
}
document.onmousedown=click;
// -->
</script>
```

