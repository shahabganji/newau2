# &#10025; Summary

An HTTP client based on the Fetch API.

| Modifier(s)                            | Extends                      | Implements                                    |
|----------------------------------------|------------------------------|-----------------------------------------------|
| export | - | - |

# &#10025; Constructor(s)

| Parameter-less                         | Implementation                          | Overload                          |
|:--------------------------------------:|:---------------------------------------:|:---------------------------------:|
| ✘ | ✔ | ✘ |

&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#10149; dom**

| Type                        | Optional                           | Rest                          | Parameter Property                          |
|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| [HTMLDOM](/runtime-html/class/dom/htmldom) | ✘  | ✘ | ✔ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Decorator(s)**

| Name                                | Decorator Factory                        |
|-------------------------------------|:----------------------------------------:|
| IDOM | ✘  |

# &#10025; Property(ies)

&nbsp;&nbsp; **&#10148; activeRequestCount**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

The current number of active requests.
Requests being processed by interceptors are considered active.

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| public | ✘ | number |

&nbsp;&nbsp; **&#10148; isRequesting**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

Indicates whether or not the client is currently making one or more requests.

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| public | ✘ | boolean |

&nbsp;&nbsp; **&#10148; isConfigured**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

Indicates whether or not the client has been configured.

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| public | ✘ | boolean |

&nbsp;&nbsp; **&#10148; baseUrl**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

The base URL set by the config.

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| public | ✘ | string |

&nbsp;&nbsp; **&#10148; defaults**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

The default request init to merge with values specified at request time.

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| public | ✘ | RequestInit &#124; null |

&nbsp;&nbsp; **&#10148; interceptors**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

The interceptors to be run during requests.

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| public | ✘ | [Interceptor](/fetch-client/interface/interfaces/interceptor)[] |

# &#10025; Method(s)

&nbsp;&nbsp; **&#10148; configure**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

Configure this client with default settings to be used by all requests.

**Parameter(s)**

| Name   | Description                                                                          |
| ------ | ------------------------------------------------------------------------------------ |
| config |  A configuration object, or a function that takes a config object and configures it. |

**Returns**

The chainable instance of this HttpClient.

**Chainable**

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| public | ✘ | [HttpClient](/fetch-client/class/http-client/httpclient) |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; config**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | RequestInit &#124; [HttpClientConfiguration](/fetch-client/class/http-client-configuration/httpclientconfiguration) &#124; ((config: HttpClientConfiguration) =&gt; HttpClientConfiguration) | ✘  | ✘ | ✘ |

&nbsp;&nbsp; **&#10148; fetch**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

Starts the process of fetching a resource. Default configuration parameters
will be applied to the Request. The constructed Request will be passed to
registered request interceptors before being sent. The Response will be passed
to registered Response interceptors before it is returned.
See also https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API

**Parameter(s)**

| Name  | Description                                                                                                    |
| ----- | -------------------------------------------------------------------------------------------------------------- |
| input |  The resource that you wish to fetch. Either a Request object, or a string containing the URL of the resource. |
| init  |  An options object containing settings to be applied to the Request.                                           |

**Returns**

A Promise for the Response from the fetch request.

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| public | ✘ | Promise&lt;Response&gt; |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; input**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | string &#124; Request | ✘  | ✘ | ✘ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; init**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | RequestInit &#124; undefined | ✔  | ✘ | ✘ |

&nbsp;&nbsp; **&#10148; buildRequest**

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| public | ✘ | Request |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; input**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | string &#124; Request | ✘  | ✘ | ✘ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; init**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | RequestInit &#124; undefined | ✘  | ✘ | ✘ |

&nbsp;&nbsp; **&#10148; get**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

Calls fetch as a GET request.

**Parameter(s)**

| Name  | Description                                                                                                    |
| ----- | -------------------------------------------------------------------------------------------------------------- |
| input |  The resource that you wish to fetch. Either a Request object, or a string containing the URL of the resource. |
| init  |  An options object containing settings to be applied to the Request.                                           |

**Returns**

A Promise for the Response from the fetch request.

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| public | ✘ | Promise&lt;Response&gt; |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; input**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | string &#124; Request | ✘  | ✘ | ✘ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; init**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | RequestInit &#124; undefined | ✔  | ✘ | ✘ |

&nbsp;&nbsp; **&#10148; post**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

Calls fetch with request method set to POST.

**Parameter(s)**

| Name  | Description                                                                                                    |
| ----- | -------------------------------------------------------------------------------------------------------------- |
| input |  The resource that you wish to fetch. Either a Request object, or a string containing the URL of the resource. |
| body  |  The body of the request.                                                                                      |
| init  |  An options object containing settings to be applied to the Request.                                           |

**Returns**

A Promise for the Response from the fetch request.

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| public | ✘ | Promise&lt;Response&gt; |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; input**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | string &#124; Request | ✘  | ✘ | ✘ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; body**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | string &#124; ArrayBuffer &#124; Blob &#124; ArrayBufferView &#124; FormData &#124; URLSearchParams &#124; ReadableStream&lt;Uint8Array&gt; &#124; undefined | ✔  | ✘ | ✘ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; init**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | RequestInit &#124; undefined | ✔  | ✘ | ✘ |

&nbsp;&nbsp; **&#10148; put**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

Calls fetch with request method set to PUT.

**Parameter(s)**

| Name  | Description                                                                                                    |
| ----- | -------------------------------------------------------------------------------------------------------------- |
| input |  The resource that you wish to fetch. Either a Request object, or a string containing the URL of the resource. |
| body  |  The body of the request.                                                                                      |
| init  |  An options object containing settings to be applied to the Request.                                           |

**Returns**

A Promise for the Response from the fetch request.

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| public | ✘ | Promise&lt;Response&gt; |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; input**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | string &#124; Request | ✘  | ✘ | ✘ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; body**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | string &#124; ArrayBuffer &#124; Blob &#124; ArrayBufferView &#124; FormData &#124; URLSearchParams &#124; ReadableStream&lt;Uint8Array&gt; &#124; undefined | ✔  | ✘ | ✘ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; init**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | RequestInit &#124; undefined | ✔  | ✘ | ✘ |

&nbsp;&nbsp; **&#10148; patch**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

Calls fetch with request method set to PATCH.

**Parameter(s)**

| Name  | Description                                                                                                    |
| ----- | -------------------------------------------------------------------------------------------------------------- |
| input |  The resource that you wish to fetch. Either a Request object, or a string containing the URL of the resource. |
| body  |  The body of the request.                                                                                      |
| init  |  An options object containing settings to be applied to the Request.                                           |

**Returns**

A Promise for the Response from the fetch request.

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| public | ✘ | Promise&lt;Response&gt; |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; input**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | string &#124; Request | ✘  | ✘ | ✘ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; body**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | string &#124; ArrayBuffer &#124; Blob &#124; ArrayBufferView &#124; FormData &#124; URLSearchParams &#124; ReadableStream&lt;Uint8Array&gt; &#124; undefined | ✔  | ✘ | ✘ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; init**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | RequestInit &#124; undefined | ✔  | ✘ | ✘ |

&nbsp;&nbsp; **&#10148; delete**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

Calls fetch with request method set to DELETE.

**Parameter(s)**

| Name  | Description                                                                                                    |
| ----- | -------------------------------------------------------------------------------------------------------------- |
| input |  The resource that you wish to fetch. Either a Request object, or a string containing the URL of the resource. |
| body  |  The body of the request.                                                                                      |
| init  |  An options object containing settings to be applied to the Request.                                           |

**Returns**

A Promise for the Response from the fetch request.

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| public | ✘ | Promise&lt;Response&gt; |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; input**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | string &#124; Request | ✘  | ✘ | ✘ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; body**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | string &#124; ArrayBuffer &#124; Blob &#124; ArrayBufferView &#124; FormData &#124; URLSearchParams &#124; ReadableStream&lt;Uint8Array&gt; &#124; undefined | ✔  | ✘ | ✘ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; init**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | RequestInit &#124; undefined | ✔  | ✘ | ✘ |

&nbsp;&nbsp; **&#10148; trackRequestStart**

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| private | ✘ | void |

&nbsp;&nbsp; **&#10148; trackRequestEnd**

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| private | ✘ | void |

&nbsp;&nbsp; **&#10148; processRequest**

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| private | ✘ | Promise&lt;Request &#124; Response&gt; |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; request**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | Request | ✘  | ✘ | ✘ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; interceptors**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | [Interceptor](/fetch-client/interface/interfaces/interceptor)[] | ✘  | ✘ | ✘ |

&nbsp;&nbsp; **&#10148; processResponse**

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| private | ✘ | Promise&lt;Request &#124; Response&gt; |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; response**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | Promise&lt;Response&gt; | ✘  | ✘ | ✘ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; interceptors**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | [Interceptor](/fetch-client/interface/interfaces/interceptor)[] | ✘  | ✘ | ✘ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; request**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | Request | ✘  | ✘ | ✘ |

&nbsp;&nbsp; **&#10148; applyInterceptors**

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| private | ✘ | Promise&lt;Request &#124; Response&gt; |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; input**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | Request &#124; Promise&lt;Request &#124; Response&gt; | ✘  | ✘ | ✘ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; interceptors**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | [Interceptor](/fetch-client/interface/interfaces/interceptor)[] &#124; undefined | ✘  | ✘ | ✘ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; successName**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | "request" &#124; "requestError" &#124; "response" &#124; "responseError" | ✘  | ✘ | ✘ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; errorName**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | "request" &#124; "requestError" &#124; "response" &#124; "responseError" | ✘  | ✘ | ✘ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; interceptorArgs**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | unknown[] | ✔  | ✔ | ✘ |

&nbsp;&nbsp; **&#10148; callFetch**

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| private | ✘ | Promise&lt;Response&gt; |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; input**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | string &#124; Request | ✘  | ✘ | ✘ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; body**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | string &#124; ArrayBuffer &#124; Blob &#124; ArrayBufferView &#124; FormData &#124; URLSearchParams &#124; ReadableStream&lt;Uint8Array&gt; &#124; undefined | ✘  | ✘ | ✘ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; init**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | RequestInit &#124; undefined | ✘  | ✘ | ✘ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; method**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | string | ✘  | ✘ | ✘ |