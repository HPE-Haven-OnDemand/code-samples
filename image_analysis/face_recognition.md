#Async

##Call
```
curl -X POST --form "apikey=<API_KEY>" --form "file=@/Users/tylernappy/hp/hp_software/devrel_samples/image_analysis/image_1.JPG" https://api.idolondemand.com/1/api/async/detectfaces/v1
```
##Return
```
{
  "jobID": "usw3p_b4a8d1d0-274c-4c1e-af87-918abb89b999"
}
```

##Check status of async
##Call
```
curl  https://api.idolondemand.com/1/job/status/<jobID>?apikey=<API_KEY>
```

##Return
```
{
  "actions": [
    {
      "result": {
        "face": [
          {
            "left": 2133,
            "top": 1975,
            "width": 72,
            "height": 72
          },
          {
            "left": 2301,
            "top": 935,
            "width": 168,
            "height": 168
          },
          {
            "left": 678,
            "top": 1743,
            "width": 200,
            "height": 200
          }
        ]
      },
      "status": "finished",
      "action": "detectfaces",
      "version": "v1"
    }
  ],
  "jobID": "usw3p_b4a8d1d0-274c-4c1e-af87-918abb89b999",
  "status": "finished"
}
```
