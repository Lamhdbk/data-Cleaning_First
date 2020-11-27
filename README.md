# data-Cleaning_First
# Often, you will find that not all the data categories in dataset are usefull for you.
# ex: you might have a dataset containing student information (name,grade,standard,parent name, and adrees)
# you want to forcus on analyzing student grade
# pandas provides a handy way of removing unwanted columns or rows from a Dataframe with the drop() function.

# let create a dataframe from csv file BL-Flickr-Images-Book.csv’
import pandas as pd
import numpy as np

# Droping column in a DataFrame

df=pd.read_csv('datasets/BL-Flickr-Images-Book.csv')
df.head()

	Identifier	Edition Statement	Place of Publication	Date of Publication	Publisher	Title	Author	Contributors	Corporate Author	Corporate Contributors	Former owner	Engraver	Issuance type	Flickr URL	Shelfmarks
0	206	NaN	London	1879 [1878]	S. Tinsley & Co.	Walter Forbes. [A novel.] By A. A	A. A.	FORBES, Walter.	NaN	NaN	NaN	NaN	monographic	http://www.flickr.com/photos/britishlibrary/ta...	British Library HMNTS 12641.b.30.
1	216	NaN	London; Virtue & Yorston	1868	Virtue & Co.	All for Greed. [A novel. The dedication signed...	A., A. A.	BLAZE DE BURY, Marie Pauline Rose - Baroness	NaN	NaN	NaN	NaN	monographic	http://www.flickr.com/photos/britishlibrary/ta...	British Library HMNTS 12626.cc.2.
2	218	NaN	London	1869	Bradbury, Evans & Co.	Love the Avenger. By the author of “All for Gr...	A., A. A.	BLAZE DE BURY, Marie Pauline Rose - Baroness	NaN	NaN	NaN	NaN	monographic	http://www.flickr.com/photos/britishlibrary/ta...	British Library HMNTS 12625.dd.1.
3	472	NaN	London	1851	James Darling	Welsh Sketches, chiefly ecclesiastical, to the...	A., E. S.	Appleyard, Ernest Silvanus.	NaN	NaN	NaN	NaN	monographic	http://www.flickr.com/photos/britishlibrary/ta...	British Library HMNTS 10369.bbb.15.
4	480	A new edition, revised, etc.	London	1857	Wertheim & Macintosh	[The World in which I live, and my place in it...	A., E. S.	BROOME, John Henry.	NaN	NaN	NaN	NaN	monographic	http://www.flickr.com/photos/britishlibrary/ta...	British Library HMNTS 9007.d.28.
