# SenateTweets

This repository is intended to be an archive of tweets gathered by the @All100Senators twitter account.

Post 02/19/17, I anticipate that data will be updated in batches of ~3k tweets. 


########## FILE FORMAT ################################################################

As of 02/19/2017, the fields available are:
Row: row number within the file
created_at: time and date of tweet	
username: user name of the posting account	
userid: user ID of account posting account	
tweet_id_str: ID of the tweet	
in_reply_to_user_id: ID of the person being replied to if any	
text: tweet content
EndColumn: special sequence to signify the end of a record

The latest files are delimited by "\t|\t": a pipe between two tabs. 
The last column (EndColumn) of each record should be "$#%". Some tweets contain endlines. 

There may be some tweets that show up in multiple files as an artifact of restarting the script to tweak the log format. I was too lazy to clean that up. All of the tweet info would be duplicate in those instances.

The older log files were tab-delimited.

########################################################################################

Some notes on the accounts being followed:

  1. The intent of the account is to aggregate the tweets of sitting US Senators.

  2. My preference is to follow 100 accounts: 1 for each Senator. But I have considered changing that. 
  
  3. Different senators may have different combinations of verified accounts corresponding to personal, Senate office, or campaign activities. Ideally, I'd prefer an account from which the Senator tweets personally on a fairly regularly basis. In some cases it isn't perfectly clear which account is the most appropriate to follow. Perhaps the constraint of only following 100 accounts is an error on my behalf.  

  4. Specific changes that have been made:
  
    Followed @BernieSanders before switching to @SenSanders 
    
    Followed @stabenow before switching to @SenStabenow
    
    Followed @ThomTillis before switching to @SenThomTillis
    
    Missed the first 7 tweets of @SenatorStrange 
