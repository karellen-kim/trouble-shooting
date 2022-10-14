# Cache
* kotlin suspend Cacheable
```kt
@Cacheable(value = ["test"])
open fun getString(id: String): Deferred<String> {
    return someScope.async {
        client.getString(id)
    }
}
```
