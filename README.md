# TopNius

Execute the script passing as parameters the inferior and superior limits:

```
python topnius.py <inferior limit> <superior limit>
```


For change the delay between requests modify DOWNLOAD_DELAY parameter in CrawlerProcess constructor. The delay will be between 0.5\*DOWNLOAD_DELAY and 1.5\*DOWNLOAD_DELAY

```
process = CrawlerProcess({
            'USER_AGENT': 'Mozilla/4.0 (compatible; MSIE 7.0; Windows NT 5.1)',
            'DOWNLOAD_DELAY': 1, #this value defines the delay between 2 requests
            'RANDOMIZE_DOWNLOAD_DELAY': True, #enables random delay between 0.5*DOWNLOAD_DELAY and 1.5*DOWNLOAD_DELAY. If it is false, the delay will be DOWNLOAD_DELAY
        })
```