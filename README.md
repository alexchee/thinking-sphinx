Thinking Sphinx
===============
This is a fork of Pat Allan's Thinking Sphinx 'v2' branch [https://github.com/pat/thinking-sphinx](https://github.com/pat/thinking-sphinx), with an extra option :ignore_connection_errors to ThinkingSphinx::Search that will silently fail on Errno::ECONNREFUSED errors if set to true.

Ex.
```
ThinkingSphinx::Search.new(:ignore_connection_errors => true)
```
This will return empty results if an Errno::ECONNREFUSED occurs.
