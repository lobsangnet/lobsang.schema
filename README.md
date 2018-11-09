# lobsang.schema

This repository serves as discussion platform to shape the JSON schema, which
serves as exchange format among all participants of Lobsang.

## Example

For now, the schema looks something like this:

```js
{
    "content": "https://www.nodeknockout.com/",
    "topic": "URL",
    "license": "GPL-3.0",
    "contentType": null,
    "created": "2018-10-31T22:03:25.785Z",
    "derivedFrom": null,
    "id": "e5dd43c3551bd...489ff2752f075d23954a10c1486ace577e4abac65df3b3ef4",
    "issuer": "Lv02OXwlrubGhWWaZs7/...ZI0yA=="
}
```

Note, that the schema will only do a loosely test for ISO8601 `created` values,
since the [strict regex][iso8601-regex] is quite large.

The test for `license` is [derived from Wikidata][spdx-regex].

## LICENSE

Apache 2.0. See [LICENSE.txt][license].

[iso8601-license]: https://stackoverflow.com/a/28022901
[license]: ./LICENSE.txt
[spdx-regex]: https://www.wikidata.org/wiki/Property:P2479
