## Leto Metrics API


- API is deployed at https://api.leto.gg/analytics (POST request with pagination support)

- We need to provide at least one cid to the api for it to work.

- Default CIDs size limit is 10, max is 50 CIDs per request (for now, can be changed if required).

Sample JSON Requests are as follows: 	

No Pagination- {
  "cids": [
    "bafkreiedazv25tc7idkywbco3jxrywdnb3g4ff3pqegrmshhtcpk5zgsyi",
    "bafkreigt25bt7a6fdnx72jhtnnoezvoihcxxlvyc6kpxkfonayxrqnpiie"
  ]
}


With Pagination-
{
  "cids": [
    "bafkreiedazv25tc7idkywbco3jxrywdnb3g4ff3pqegrmshhtcpk5zgsyi",
    "bafkreigt25bt7a6fdnx72jhtnnoezvoihcxxlvyc6kpxkfonayxrqnpiie"
  ],
  "page": 1,
  "size": 5
}

Make the request to https://api.leto.gg/analytics 
