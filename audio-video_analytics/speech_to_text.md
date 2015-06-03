#Async

##Call
```
curl -X POST --form "apikey=<API_KEY>" --form "file=@/Users/tylernappy/Downloads/SampleVideo_1080x720_1mb.mp4" https://api.idolondemand.com/1/api/async/recognizespeech/v1
```
##Return
```
{
  "jobID": "usw3p_2ec34811-7d8d-4947-b2ec-062b0b466412"
}
```


##Check status of async
##Call
```
curl  https://api.idolondemand.om/1/job/status/<jobID>?apikey=<API_KEY>
```

##Return
```
{
  "actions": [
    {
      "result": {
        "document": [
          {
            "content": "mm"
          }
        ]
      },
      "status": "finished",
      "action": "recognizespeech",
      "version": "v1"
    }
  ],
  "jobID": "usw3p_2ec34811-7d8d-4947-b2ec-062b0b466412",
  "status": "finished"
}
```
