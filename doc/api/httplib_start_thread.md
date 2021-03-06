# LibHTTP API Reference

### `httplib_start_thread( func, cbdata );`

### Parameters

| Parameter | Type | Description |
| :--- | :--- | :--- |
|**`func`**|`httplib_thread_func_t`|Function to start as a separate thread|
|**`cbdata`**|`void *`|User defined data to be passed to the thread as parameter|

`void httplib_thread_func_t( void *cbdata );`

### Return Value

| Type | Description |
| :--- | :--- |
|`int`|Success or error code|

### Description

The function `httplib_start_thread()` is a convenience function to create a detached thread. The function returns **0** when successful and another value if an error occured. A pointer to user supplied data can be passed which is then passed further on to the thread function as parameter.

### See Also

* [`httplib_start();`](httplib_start.md)
