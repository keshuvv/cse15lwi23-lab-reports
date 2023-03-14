# Lab Report 5 

## For this lab report, I have chosen the `find` command. Following are some of the command line options for `find` that I found interesting:_ 

## 1. `-size n` option 
   * Description: 
                  [Source](https://man7.org/linux/man-pages/man1/find.1.html)
                  
   * Example 1: ![Image](images/size+1.png)
   * Example 2: ![Image](images/size+2.png)
   
## 2. `-type ` option 
   * Description: 
                  [Source](https://man7.org/linux/man-pages/man1/find.1.html)
        
   * Example 1: ![Image](images/type-d.png)
   * Example 2: ![Image](images/type-f.png)
  

## 3. `-empty ` option
   *  Description: This command-line option is used to find the files/directories that are empty, i.e. have no content. [Source](https://man7.org/linux/man-pages/man1/find.1.html)
           
   * Example 1: For the first example, I tried finding all the empty files within the ./witten_2 directory. The command that I used for the same was: `find ./written_2 -type f -empty`. Here, I am also using the previous command-line option `type` to define that I am strictly interested in findig empty 'files' and not directories, etc. 
   * The result I obtained for this was that there were no empty files in the directory that I had passed. Please refer to the following screenshot to see the implementation of this example and the result I obtained. ![Image](images/empty-f.png)
 
   * Example 2: For the second example, I wanted to find all the empty directories within the ./witten_2 directory. The command that I used for the same was: `find ./written_2 -type d -empty`. 
   * It again gave me no result, which meant that there were no empty directories either. ![Image](images/no.png)
   * To verify the working of this command-line option, I created two empty directories within the `./wirtten_2` directory by using these commands: `mkdir ./written_2/new_directory`, `mkdir ./written_2/new_folder`. Now, this time when I passed the `find ./written_2 -type d -empty` command again, I got the list of empty directories. Please refer to the following screenshot to see the implementation of this example and the result I obtained. ![Image](images/empty-d.png)

## 4. `-links n` option
   * Description: This command-line option is used to find the files based on the number of hard links that point to them. [Source](https://man7.org/linux/man-pages/man1/find.1.html)
           
   * Example 1: For the first example, I tried finding all the files within the ./witten_2 directory with exactly 5 hard links. The command that I used for the same was: `find ./written_2 -links 5`. Please refer to the following screenshot to see the implementation of this example and the result I obtained. ![Image](images/links-5.png)
   * Example 2: For the first example, I was curious to find all the files within the ./witten_2 directory with more than 5 hard links. The command that I used for the same was: `find ./written_2 -links +5`. Please refer to the following screenshot to see the implementation of this example and the result I obtained. ![Image](images/links+5.png)
 
***Thank you for reviewing my lab report, appreciate it!*** 
