---
name: Add the language used for the audio track to AudioAttributes
about: Add to AudioAttributes the camp AudioLanguage
title: 'Add to AudioAttributes the camp AudioLanguage'
labels: 'enhancement'
assignees: 'development team'

---

**Is your feature request related to a problem? Please describe.**

The UK video-on-demand client emailed us about additional metadata that they want to store in Movida and then publish to YouView for new content to publish in their platform.

**Describe the solution you'd like**
The current xml format presents the minimal metadata requirement 8.1.3.1 from the 4300-CP document.

<AVAttributes>
<AudioAttributes>
<MixType href="urn:mp

The solution is to add AudioLanguage attribute to it ( 8.1.4 from the 4300-CP document).
For this we need to add this parameter to the tables on the database and store the values from the client.

The section 8.2.3.2 from the 4300-CP document shows an example for the solution:
<AudioAttributes>
<MixType href="urn:mpeg:mpeg7:cs:AudioPresentationCS:2001:5"/> 
<AudioLanguage type="original" supplemental="false"
purpose="urn:tva:metadata:cs:AudioPurposeCS:2007:6">en</AudioLanguage> 
</AudioAttributes>
