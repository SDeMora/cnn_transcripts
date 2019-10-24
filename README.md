## CNN Transcripts 

**For copyright reasons, access is restricted for research purposes only.**

**Forked from: [/notnews/cnn_transcripts](https://github.com/notnews/cnn_transcripts)**


CNN provides transcripts for its shows at [http://edition.cnn.com/TRANSCRIPTS/](http://edition.cnn.com/TRANSCRIPTS/). 

The transcripts are available for shows starting `1999/10/01`. See [http://edition.cnn.com/TRANSCRIPTS/1999.10.01.html](http://edition.cnn.com/TRANSCRIPTS/1999.10.01.html). However, we get a 'Page not found' error when we follow links until `1999/12/31`. So we started scraping the data from `2000/01/01`.

CNN went through a few HTML styles of the news transcripts between `2000/01/01`and 2014. So there are two scapers to parse the different HTML styles:

* [till 2002/9/17](scripts/cnn-1.py)
* [from 2002/9/17](scripts/cnn-2.py)

This new script scrapes and exports all data after the last point on Dataverse. It is the same as [cnn-2.py](scripts/cnn-2.py), but with an updated start date.

* [from 2014/06/18](scripts/cnn-3.py)

### Data

The parsed data are posted at [http://dx.doi.org/10.7910/DVN/ISDPJU](http://dx.doi.org/10.7910/DVN/ISDPJU). **For copyright reasons, access is restricted for research purposes only.** The data are split into 6 files:

* `cnn-1.csv`. Data from 2000/01/01--2000/04/20. No. of transcripts = 7,017
* `cnn-2.csv`. Data from  2000/04/21--2001/04/03. No. of transcripts = 21,381
* `cnn-3.csv`. Data from  2001/04/04--2002/08/06. No. of transcripts = 35,269
* `cnn-4.csv`. Data from  2002/08/07--2002/09/16. No. of transcripts = 2,343
* `cnn-5.csv`. Data from  2002/09/17--2012/05/18. No. of transcripts = 101,336
* `cnn-6.csv`. Data from  2012/05/19--2014/06/17. No. of transcripts = 23,536

Total number of transcripts: 190,882

If we add in transcripts after 2014/06/18 (the last Dataverse data point) we get:

* `cnn-7.csv`. Data from  2014/06/18--2019/08/22. No. of transcripts = 54,960

Total number of transcripts: 245,842



NOTES:

Scripts work in Python 2.7
