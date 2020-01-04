# &#10025; Summary

A class for configuring HttpClients.

| Modifier(s)                            | Extends                      | Implements                                    |
|----------------------------------------|------------------------------|-----------------------------------------------|
| export | - | - |

# &#10025; Property(ies)

&nbsp;&nbsp; **&#10148; baseUrl**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

The base URL to be prepended to each Request's url before sending.

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| public | ✘ | string |

&nbsp;&nbsp; **&#10148; defaults**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

Default values to apply to init objects when creating Requests. Note that
defaults cannot be applied when Request objects are manually created because
Request provides its own defaults and discards the original init object.
See also https://developer.mozilla.org/en-US/docs/Web/API/Request/Request

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| public | ✘ | RequestInit |

&nbsp;&nbsp; **&#10148; interceptors**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

Interceptors to be added to the HttpClient.

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| public | ✘ | [Interceptor](/fetch-client/interface/interfaces/interceptor)[] |

# &#10025; Method(s)

&nbsp;&nbsp; **&#10148; withBaseUrl**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

Sets the baseUrl.

**Parameter(s)**

| Name    | Description    |
| ------- | -------------- |
| baseUrl |  The base URL. |

**Returns**

The chainable instance of this configuration object.

**Chainable**

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| public | ✘ | [HttpClientConfiguration](/fetch-client/class/http-client-configuration/httpclientconfiguration) |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; baseUrl**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | string | ✘  | ✘ | ✘ |

&nbsp;&nbsp; **&#10148; withDefaults**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

Sets the defaults.

**Parameter(s)**

| Name     | Description    |
| -------- | -------------- |
| defaults |  The defaults. |

**Returns**

The chainable instance of this configuration object.

**Chainable**

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| public | ✘ | [HttpClientConfiguration](/fetch-client/class/http-client-configuration/httpclientconfiguration) |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; defaults**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | RequestInit | ✘  | ✘ | ✘ |

&nbsp;&nbsp; **&#10148; withInterceptor**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

Adds an interceptor to be run on all requests or responses.

**Parameter(s)**

| Name        | Description                                                                                                                                                                                                                                                                          |
| ----------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| interceptor |  An object with request, requestError, response, or responseError methods. request and requestError act as resolve and reject handlers for the Request before it is sent. response and responseError act as resolve and reject handlers for the Response after it has been received. |

**Returns**

The chainable instance of this configuration object.

**Chainable**

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| public | ✘ | [HttpClientConfiguration](/fetch-client/class/http-client-configuration/httpclientconfiguration) |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; interceptor**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | [Interceptor](/fetch-client/interface/interfaces/interceptor) | ✘  | ✘ | ✘ |

&nbsp;&nbsp; **&#10148; useStandardConfiguration**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

Applies a configuration that addresses common application needs, including
configuring same-origin credentials, and using rejectErrorResponses.

**Returns**

The chainable instance of this configuration object.

**Chainable**

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| public | ✘ | [HttpClientConfiguration](/fetch-client/class/http-client-configuration/httpclientconfiguration) |

&nbsp;&nbsp; **&#10148; rejectErrorResponses**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

Causes Responses whose status codes fall outside the range 200-299 to reject.
The fetch API only rejects on network errors or other conditions that prevent
the request from completing, meaning consumers must inspect Response.ok in the
Promise continuation to determine if the server responded with a success code.
This method adds a response interceptor that causes Responses with error codes
to be rejected, which is common behavior in HTTP client libraries.

**Returns**

The chainable instance of this configuration object.

**Chainable**

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| public | ✘ | [HttpClientConfiguration](/fetch-client/class/http-client-configuration/httpclientconfiguration) |

&nbsp;&nbsp; **&#10148; withRetry**

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| public | ✘ | [HttpClientConfiguration](/fetch-client/class/http-client-configuration/httpclientconfiguration) |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; config**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | [RetryConfiguration](/fetch-client/interface/interfaces/retryconfiguration) &#124; undefined | ✔  | ✘ | ✘ |