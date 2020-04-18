1. Say one developer is developing the DAST software so he has written a vulnerable app, now in second iteration another developer might 
need to write one more vulnerable application as previously written app is not there anymore and reviewers need to understand how to use 
new app too.

Writing one more vulnerable app is not tough as springboot makes things very easy but still finding all the dependencies, creating UI
creating backend logic everything might require one day effort and with vulnerable app it might be reduced to 2-3 hour and if 
say any other DAST already has covered that vulnerability then it doesn't require any time to check the payloads also in case 
already a vulnerability is added to vulnerableApplication then adding new payload/new level doesn't require modification
to pom.xml or basic UI layout etc.

For reviewers learning one vulnerable app and then using it can be very easy and they need not to install multiple vulnerable applications
May be installing multiple webapplications might not be tough but as these steps are tedious so they need not to do.

2. Custom written vulnerable apps might be buggy and there is no certainty that they are written properly. For reviewers 
of DAST payloads to look into the Custom vulnerable app is very difficult so with one vulnerable application which 
is maintained by community has more chances of not having bugs.
