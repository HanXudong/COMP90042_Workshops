# COMP90042_Workshops
## Tutor
- Name: Xudong Han
- Email: xudong.han@unimelb.edu.au

## Week 5
Still working on it...

## Week 4
- Logarithmic index layout: <br>
	http://2048game.com/
- Logarithmic index layout I/Os treadoff <br>
Question: will the Log index require higher I/O resource consumption for IR?<br>
My idea: No. When processing a certain query, all rows in every Inverted Index which are related to query terms will be read to RAM. In this case, no matter how many indexes are stored in the disk, the total amount of data transmitted is the same. The difference might be the seek time. When doing a disk read or write, it takes a while for the disk head to move to the part of the disk where the data are located. This time is called the seek time and it averages 5 ms for typical disks. If indexes are stored in different parts, a long seek time will be the problem. However, solid state disk has been widely used and typical SSDs will have a seek time between 0.08 and 0.16 ms. Such that, even a large number of indexes are used by logarithmic index layout, the I/Os requirement of it is almost the same as one big index structure.
- Data types:<br>
	https://docs.scipy.org/doc/numpy-1.10.1/user/basics.types.html
