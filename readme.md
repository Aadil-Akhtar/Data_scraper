

## Created by     
## Debartha Chakraborty                |               Aadil Akhtar
    debartha2riki@gmail.com       | Aadil.Akhtar.ph120@physics.iitd.ac.in
    
   [Debartha's LinkedIn]( https://www.linkedin.com/in/debartha-chakraborty-77190620a)                                                                                                                                      |        [Aadil's LinkedIn](https://www.linkedin.com/in/aadil-akhtar-549297213/)


**metadata.csv** in the source file where there are two cloumns:- 
- First one is the movie ID in IMDB site.



- Second one is the name of the movie. 
     >we are only using the first column in the code



     
**imdb_data.csv** is the output file where all the scraped data gets stored.

If you want to scrape all the data at one single run, change the value of the variable `end` to `len(mainlist)` in the  **multithread.&#8204;py** file and run the file.

&nbsp;



`end = len(mainlist)`

 >change this to the number of pages you want to scrape

If you want to scrape your data in smaller batches (say 1000), change the value of the variable `end` to the batch size (i.e. 1000) in the **multithread.&#8204;py** file then run the code using  **run.&#8204;py**

However you can change the value of `max_workers` to the suitable number that your computer can handle easily. 
>4 to 8 workers are normally stable.

  
  `with concurrent.futures.ThreadPoolExecutor(max_workers=4) as executor:`