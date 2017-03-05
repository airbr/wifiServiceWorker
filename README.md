### Offline Demo instructions

1. clone the repo
2. run `http-server` or similar in the repo folder
3. Visit localhost:8080 or whatever
4. See regular content on page, service worker info in console
5. kill `http-server`
6. refresh localhost:8080
7. See cached offline page instead of browser version

### "Online Offline" (zounds!) Demo instructions:

1. Go to [https://wifiserviceworker.firebaseapp.com/](https://wifiserviceworker.firebaseapp.com/) which should give you a re-assuring message that you are online.
2. Disconnect your internet connection. Give the website a 'normal' or 'soft' refresh. It will likely remain the same due to being cached*.
3. Give the website a [hard refresh](http://refreshyourcache.com/en/cache/) i.e:
  
	* Windows: ctrl + F5
	* Mac/Apple: Apple + R or command + R
	* Linux: F5


4. You will likely see a message saying it cannot load the page because of no internet connection upon doing this the first time as you clear the cache. Do not be afraid! open a new tab and visit that URL again and you should see offline page with a comforting orange background. Magic!
 
 
 
---

### Project Status: Offline is Online :ballot_box_with_check:

A project to meet the 'lighthouse audit test' of [a URL that responds with a 200 when offline](https://developers.google.com/web/tools/lighthouse/audits/http-200-when-offline) and also gives some kind of visual responsive cue to the user that that would seem as if they are in fact online.

Intended to be a re-usable module basically to add some kind of customizable failing view so that a user never see's the failasaur or equivalent anymore:

![Failasaur](https://qph.ec.quoracdn.net/main-qimg-2726194a5aea31c692cc6ccb06457469)



## Resources

[Simple Service Worker Tutorial](https://github.com/airbr/simple-serviceworker-tutorial)

[Progressive Web Apps across all frameworks - Google I/O 2016
](https://www.youtube.com/watch?v=srdKq0DckXQ)

[Future App Model: Advanced Service Worker (Chrome Dev Summit 2016)
](https://www.youtube.com/watch?v=J2dOTKBoTL4&t=305s)

[MDN service worker basic example](https://github.com/mdn/sw-test)

[Offline Fallback recipe](https://serviceworke.rs/offline-fallback.html)
