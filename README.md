# Opera Roles Recommender


## Summary

This tool will take a list of opera roles a singer has previously sung, and generate a list of further roles in the repertoire which the user might enjoy/be able to perform. It can take input from lists of roles performed by other singers who have sung multiple roles, generated from singer biographies, potentially also from programme notes and from reviews.  Building AI course project.


## Background

The scope of all opera roles is large, even when restricted by the slightly crude filter of 'voice-type'.  Amateur opera singers in particular are often unaware of particular roles that might well suit them to sing.  Even singing teachers and other colleagues will tend to only recommend roles from the best-known operas, limiting an individual's horizon of what could be possible for them.


## How is it used?

The user will input a list of roles they have sung.  The AI will return a recommended list of further roles with links to descriptions and recordings.


## Data sources and AI methods

The AI will build up a database of opera roles ([Wikipedia](https://en.wikipedia.org/wiki/Main_Page) might be a good start, cross-checked with [Oxford Music Online](https://www.oxfordmusiconline.com/page/1805)), and then of soloists who've sung multiple roles.  This second step would require a search of opera singers ([Ranker](https://www.ranker.com) (search for 'List of Famous Opera Singers') might be a good source), and then for each singer a scan of their biographies  or other online material to identify their roles sung.

The AI would then match the roles sung by the user with 'nearest neighbours' in the opera singers lists of roles sung.  While the usual filter of voice-type (soprano, alto, etc) might appear to largely impact the results, many singers can and have sung roles across these boundaries.  So the AI by design would not specifically use voice-type, and would just focus on roles sung.


## Challenges

We'll need a way to uniquely identify each opera role.  It might be necessary to frame them as data-pairs of Opera-name/Role-name for disambiguation.

Building the database of roles sung by a large number of singers looks to be a significant challenge.  There doesn't appear to be a single resource online for this.  And reading 'biographies' or 'reviews' may identify roles by names other than those in our master list, due to language for instance.


## What next?

Once built, an obvious extension would be to help the user identify possible opportunities to sing this role.  This would require some kind of structured search of relevant performing groups within a geographic space, and possibly setting up alerts for when those roles come up.  There is a somewhat limited auditions listing resource ([Audition Oracle](https://auditionoracle.com/auditions/?rbj=y)) that might also be used.


## Acknowledgments

Reaktor and University of Helsinki for creating the [Elements of AI](https://course.elementsofai.com/) and [Building AI courses](https://buildingai.elementsofai.com/).
