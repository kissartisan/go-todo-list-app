### Gotchas on learning
- Following the tutorial, I ended up manually changing the `Access-Control-Allow-Origin` and `Access-Control-Allow-Methods` headers to allow access origin
- There's an `OPTION` method request  that was called before hitting the `DELETE` method  request. I'm still unsure why.
  - This ends up having a log of `TodoItem not found in database` since the delete function was called twice (one for `OPTION` request and one for `DELETE` request)
