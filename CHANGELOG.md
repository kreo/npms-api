# Changelog


# v2.0.0 - 2016-09-19

- Changed `?term` to `?q` in `/search`, which now supports [qualifiers](https://api-docs.npms.io/#api-search-query) to filter and modify results
- Changed `?term` to `?q` in `/search/suggestions`
- Removed `scoreEffect`, `qualityWeight`, `maintenanceWeight` and `popularityWeight` query parameters from `/search` in favor of qualifiers
- Changed `/module` to `/package`
- Changed `module` to `package` in every response
- Added `flags` to the search & suggestions responses
- Response structure of `/package` and `/package/mget` changed because the `npms-analyzer` analysis structure also changed

This new API is available under `https://api.npms.io/v2`.

The `v1` is deprecated and will be removed on 2016-12-19.
Until then `https://api.npms.io` will still point to `v1`. Afterwards, it will always point to the latest API version.   
Also the `v1` API data will be stale, which means that the newest packages and updates won't be available.


# v1.0.0

Initial release.

This new API is available under `https://api.npms.io/v1`.
