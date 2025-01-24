# Common HTTP Method Override Parameters

Here are some commonly used parameter names that you can manually try or include in your fuzzing tools:

- `_method`
- `_method_override`
- `_methodType`
- `_methodName`
- `_override`
- `_http_method`
- `_httpMethod`
- `_requestMethod`
- `_xmethod`
- `_action`
- `_verb`
- `_type`
- `_op`
- `_func`
- `_requesttype`

## Example Usage with FFUF

You can use the following command to test for HTTP method override vulnerabilities:

```bash
ffuf -u "http://example.com/resource?FUZZ=POST" -w SecLists/Discovery/Web-Content/burp-parameter-names.txt -X GET
