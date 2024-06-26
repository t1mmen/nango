# Changelog

All notable changes to this project will be documented in this file.

## [0.39.28] - 2024-05-15

### Added

- *(db)* Add ability to change schema name (#2126)
- *(orchestration)* Introducing the scheduler (#2132)
- *(db)* Add extensions to search_path (#2143)
- *(webapp)* [nan-839] add secondary url (#2135)
- [nan-851] improve query to use the nango_config_id (#2124)
- *(logs)* GET /logs/operations/:operationId (#2156)
- *(cli)* [nan-918] exit deploy if not everything compiled successfully (#2158)

### Fixed

- *(action)* Logs ActionError in activities (#2148)
- *(db)* Backfill secret key hash (#2134)
- *(action)* Log all errors
- *(env)* Correctly parse db-schemas (#2154)
- *(oauth)* [nan-934] fix public key lookup (#2157)
- *(ui)* Env switching issue (#2152)
- *(webapp)* [nan-943] fix API reference for multi models (#2159)

## [v0.39.27] - 2024-05-13

### Added

- *(logs)* Add more context #2 (#2146)
- *(ui)* Logs search mvp  (#2106)

### Fixed

- *(release)* Improve changelog (#2147)

## [v0.39.26] - 2024-05-13

### Fixed

- *(schedule)* Add scheduleId and warn label (#2142)
- *(schedule)* Comparison when checking if a schedule is paused (#2144)
- *(release)* Publish correctly to github (#2141)

## [v0.39.25] - 2024-05-10

### Added

- *(integrations)* Add support for dialpad (#2082)
- *(logs)* POST /logs/search (#2063)
- *(debug)* Add more details when pausing temporal schedule (#2139)
- *(sdk)* Add more caching (#2111)
- *(metrics)* [NAN-664] track more usage metrics in datadog (#2136)

### Changed

- Remove heroku/render from self-hosted guides (#2110)
- Better Result types (#2116)
- Publish missing main package version in lock (#2138)

### Fixed

- *(release)* Automatic release publishing (#2103)
- *(server)* Remove list schedules (#2137)
- *(sdk)* Logging null breaks script (#2140)

## [v0.39.24] - 2024-05-10

### Added

- *(oauth2cc)* Add authorization request parameters (#2053)
- *(logs)* Add more context data (#2034)
- *(integrations)* Add support for posthog api (#2102)
- *(integrations)* Add support for wealthbox (#2109)
- *(auth)* Add span and cache 🙈 (#2114)
- *(persist)* Add error details in auth.middleware (#2113)
- *(integrations)* Add support for lessonly api (#2083)
- *(integrations)* Add support for envoy api (#2092)
- *(integration)* Add strava-web-oauth integration (#2118)
- *(integration)* Add Bland.ai (#2098)
- *(integrations)* Add support for pivotaltracker api (#2084)

### Changed

- Script to migrate records (#1934)
- No cap (#2104)
- *(deps)* Bump ejs from 3.1.9 to 3.1.10 (#2078)

### Fixed

- *(persist)* Truncate big logs (#2074)
- *(api)* Handle 404 as json (#2085)
- *(db)* Slow query getSyncs (#2088)
- *(api)* Setup for e2e tests (#2090)
- *(Provider)* Proxy is optional (#2096)
- *(docker)* Set correct platform (#2101)
- *(logs)* Make it completely optional (#2100)
- *(api)* Unified context (#2097)
- Latency and type error (#2112)
- Ensure secret_key_hashed is updated when needed (#2119)
- Set secret_key_hashed when creating environment (#2122)
- Show error details from persist in activity logs (#2129)

## [v0.39.23] - 2024-05-01

### Added

- Add authentication (#2076)

### Changed

- Return new upsert result + retry upsert (#2079)

## [v0.39.22] - 2024-05-01

### Fixed

- *(eslint)* Pass #11 (#2058)

## [v0.39.21] - 2024-04-30

### Added

- Types package (#2055)

## [v0.39.20] - 2024-04-30

### Added

- *(integrations)* Add support for pingboard api (#2052)
- *(integrations)* Add support for squarespace (#2031)

### Changed

- *(pkg)* Dirty release commit (#2056)

### Fixed

- *(sync)* Maximum call stack for large dataset (#2064)

## [v0.39.19] - 2024-04-29

### Added

- *(integration)* Add support for google docs api (#1967)
- *(integration)* Add support for kustomer (#1958)
- *(sdks)* Document frontend and node sdks in code (#1984)
- *(db)* Add public to search_path (#2002)
- *(ci)* Add eslint (#2007)
- *(integrations)* Add support for refiner (#2009)
- Add temporal ui to docker-compose (#2006)
- *(integration)* Add api support for insightly (#2028)
- *(integration)* Add api support for freshsales (#2027)
- Hn demo (#2041)
- *(logs)* Implem v2 logging (#1945)
- *(integrations)* Add support for klipfolio api (#2038)
- *(integrations)* Add support for harvest api (#2039)
- *(integrations)* Add support for egnyte api (#2044)
- *(integrations)* Add support for expensify api (#2047)

### Changed

- Correct default action HTTP method
- Sample app (#2008)
- Sample app feedback (#2013)
- Improve Microsoft OAuth docs

### Fixed

- *(npm)* Use ci instead of install (#1988)
- *(webhooks)* Do not await send (#1977)
- *(node)* Use version 20 (#1989)
- *(api)* Only enable session for web (#1994)
- *(integration)* Use random id on conflict (#1997)
- *(api)* Stop using env cookie (#1987)
- Type of count is a string (#2005)
- *(ci)* Eslint (#2011)
- *(utils)* Move metrics (#2012)
- Logs don't show the context when detecting records differences (#2018)
- 'localeCompare is not a function' error (#2020)
- Set same deletedAt/updatedAt for deleted records in the same batch (#2021)
- *(ui)* Handle long entity names (#2019)
- Swap links in webhooks doc page (#2022)
- BatchDelete counts already deleted records or non-existing ones as deleted (#2023)
- *(api)* Wrong join for getSyncs (#2029)
- *(release)* Unify build  (#2026)
- Docker compose  (#2043)
- *(error)* Use stringifier (#2042)
- *(records)* Transaction not reusing opened connection (#2045)
- *(logs)* Wrong zod coerce, add tracer (#2046)
- *(logs)* Missing contextGetter in syncCommand (#2049)
- *(envs)* Allow empty string (#2050)
- *(ui)* Remove HN special login (#2057)
- *(logs)* Only require envs for cloud (#2060)

## [v0.39.18] - 2024-04-11

### Fixed

- *(node)* Missing type for webhook (#1982)

## [v0.39.17] - 2024-04-11

### Changed

- *(deps-dev)* Bump vite from 4.5.2 to 4.5.3 (#1948)
- *(deps)* Bump undici from 6.6.2 to 6.11.1 (#1955)

### Fixed

- *(webhooks)* Expose type, fix docs, verifyWebhookSignature helper (#1976)
- *(integration)* Simple fix for peopledatalabs api support (#1964)
- Fix heartbeat (#1980)
- TypeError: request.headers.split is not a function (#1981)

## [v0.39.16] - 2024-04-10

### Added

- Logs storage v2 (#1865)
- *(utils)* Add barrel file (#1947)
- *(integrations)* Api support for snowflake (#1962)

### Changed

- *(deps-dev)* Bump webpack-dev-middleware from 5.3.3 to 5.3.4 (#1897)
- *(deps)* Bump express from 4.18.2 to 4.19.2 (#1914)
- Report high memory usage (#1943)

### Fixed

- *(eslint)* Pass #9 (#1928)
- *(ui)* Correct 404 (#1935)
- *(ui)* Sync cookie and url (#1921)
- *(demo)* Server side tracking (#1936)
- *(login)* Correct accountId (#1939)
- *(docker)* Change Postgres version for public docker-compose (#1942)
- Use destructured object on some functions (#1941)
- Remove to getAccountUUIDFromEnvironment (#1944)
- Do not idle runner if idleMaxDurationMs is 0 (#1949)
- *(eslint)* Pass #10 (#1951)
- *(sync)* VerifyOwnership not awaited (#1952)
- *(error)* Reuse errors definition (#1954)
- *(proxy)* DryRun optional activityLogId (#1959)
- *(demo)* Move step_1 success tracking after the frontend auth (#1961)
- *(providers)* Wave accounting token url (#1966)
- *(node)* Wrong casing for modified_after (#1972)
- *(node)* Proper types for listRecords and deprecate delta (#1973)
- *(node)* Wrong condition on delta (#1974)

## [v0.39.14] - 2024-04-01

### Fixed

- *(ui)* Environment settings title (#1920)
- *(utils)* Parse env with zod (#1919)
- *(deps)* Pin redis (#1925)

## [v0.39.13] - 2024-03-28

### Added

- *(demo)* Add more backend tracking (#1912)

### Fixed

- *(env)* Re-enable dynamic key (#1899)
- *(ui)* Always identify to posthog (#1900)
- *(demo)* Feedbacks (#1901)
- *(ui)* Hmac issues (#1902)
- *(ui)* Improve cache for session, integrations (#1904)
- BatchDelete returns incorrect sync result (#1907)
- *(api)* Get env by secretKey (#1908)
- *(env)* Pin Postgres (#1915)

## [v0.37.0] - 2024-03-22

### Fixed

- *(env)* Unsafe getEnvByName (#1896)
- *(flows)* Path + strictness (#1894)

## [v0.39.8] - 2024-03-21

### Fixed

- *(cli)* Glob change of behavior (#1891)

## [v0.39.7] - 2024-03-21

### Fixed

- *(shared)* Specify published files (#1890)

## [v0.39.6] - 2024-03-21

### Added

- Add helpers to vitest (#1869)
- *(integration)* Add integration templates for zoho-mail (#1857)

### Changed

- *(deps)* Bump follow-redirects from 1.15.4 to 1.15.6 (#1864)
- Unified dockerfile (#1840)
- Remove node 19 (#1883)

### Fixed

- *(deps)* Upgrade knex (#1868)
- *(integrations)* Backfill integration templates (#1833)
- Prevent race condition when updating job results (#1867)
- *(eslint)* Pass #6 (#1871)
- *(eslint)* Pass #7 (#1874)
- Deleting lots of records (track_deletes=true) (#1878)
- *(ui)* Env not updating (#1880)
- *(flows)* Enforce compilation (#1881)
- Integration should be unique per environment (#1889)
- *(eslint)* Pass #8 (#1882)
- *(shared)* Proper ts rootDir (#1887)

## [v0.39.5] - 2024-03-15

### Added

- *(integration)* Add support for lever-basic-sandbox (#1848)

### Fixed

- *(demo)* Feedback (#1855)
- Fix flaky regex (#1859)
- *(demo)* Hide after complete (#1849)
- *(demo)* Feedback 2 (#1860)
- *(activity)* Logs order (#1861)

## [v0.39.4] - 2024-03-14

### Fixed

- *(eslint)* Pass #5 (#1846)
- *(webapp)* Fix copy button value (#1847)
- *(jobs)* Do not wait for temporal (#1850)
- Fix flaky test (#1853)
- *(demo)* Pause new demo (#1851)
- *(ui)* Use hooks for meta/env/user (#1844)

## [v0.39.3] - 2024-03-13

### Added

- Interactive demo (#1801)

## [v0.39.2] - 2024-03-13

### Added

- Show debug mode in UI (#1831)
- *(ui)* Add cn() utils (#1835)
- *(flows)* Add github issues demo example flow (#1834)
- *(eslint)* Add lint-staged (#1843)

### Fixed

- *(demo)* Missing input (#1837)
- *(auth)* Correctly save debug mode in session (#1838)
- Eslint #4 (#1842)

## [v0.39.1] - 2024-03-08

### Added

- *(webapp)* Improve on scopes input fields and download flow (#1794)

### Fixed

- Nango deps version and publish.sh (#1821)
- *(deps)* Pin aws-sdk (#1826)

## [v0.39.0] - 2024-03-07

### Added

- *(integrations)* Api support for teamtailor (#1747)
- *(integrations)* Integration template for teamtailor (#1748)
- *(webapp)* Improve field values on refresh (#1782)
- *(db)* Add index for isSyncJobRunning (#1793)
- *(integrations)* Api support and integration template for zoho-mail (#1779)
- *(SecretInput)* Handle null optionalvalue gracefully (#1781)
- *(webapp)* Improve input integration ID on edit (#1783)

### Changed

- *(eslint)* --fix #3 (#1798)
- *(deps-dev)* Bump posthog-js from 1.51.4 to 1.57.2 (#1819)

### Fixed

- *(db)* Missing index on records (#1769)
- *(lint)* Enable type checker (#1756)
- *(cron)* Delete syncs naive approach (#1776)
- *(datadog)* Correctly track runner (#1766)
- *(db)* Clean up indexes (#1787)
- *(dd)* Wrong import in server (#1789)
- *(integration)* Stripe-app access token refresh on expire (#1780)
- *(manifest)* Fix property names (#1795)
- Jobs vulnerability (#1799)
- *(eslint)* Improve webapp reporting (#1804)
- *(getting-started)* Remove some code snippets, re-up local testing (#1803)
- *(integration)* Teamtailor integration sync template (#1816)
- *(ui)* Remove top nav logout (#1809)
- *(ui)* Move and pin devDependencies (#1808)

## [v0.38.5] - 2024-02-29

### Added

- *(integrations)* Api support for pinterest (#1738)
- *(integrations)* Api support for anrok (#1739)
- *(ui)* Merge with npm workspace (#1735)

### Fixed

- *(db)* Remove schema() (#1746)
- *(deploy)* Correctly output error and end the activity (#1757)
- *(sync)* Off-load data deletion (#1745)

## [v0.38.4] - 2024-02-27

### Changed

- *(deps)* Bump es5-ext from 0.10.62 to 0.10.63 (#1750)

### Fixed

- *(test)* Update tests (#1749)
- *(connection)* Empty creds when deleting (#1743)
- *(node)* Expose all types (#1751)
- *(cli)* Compiler should skip project (#1752)

## [v0.38.3] - 2024-02-26

### Changed

- *(deps)* Bump ip from 1.1.8 to 1.1.9 (#1711)

## [v0.38.2] - 2024-02-26

### Added

- *(db)* Add index for getAddedKeys() (#1732)
- *(db)* Add index for connections (#1733)
- *(db)* Add search path (#1727)

### Fixed

- *(server)* Handle undefined status code (#1737)
- *(sync)* Await full cancel (#1740)

## [v0.38.1] - 2024-02-23

### Added

- Add total records count and size metrics (#1725)

### Changed

- Eslint --fix (#1712)

### Fixed

- *(db)* Remove unnecessary groupBy (#1723)
- *(nango_sync_endpoints)* Relationship doesn't exist (#1731)

## [v0.38.0] - 2024-02-23

### Added

- *(db)* Add index for logs (#1721)
- *(db)* Add index for sync_jobs (#1717)
- *(db)* Add index for data_records (#1719)
- *(db)* Add index to configs (#1724)

## [v0.37.26] - 2024-02-22

### Changed

- Temporal activities timeout (#1720)

### Fixed

- Use GET /config/KEY to obtain provider in cli dryrun (#1722)

## [v0.37.25] - 2024-02-22

### Added

- *(integrations)* Add support and integration for nextcloud (#1635)
- *(integrations)* Add integration templates for ashby (#1637)
- *(sdk)* Add optional telemetry (#1683)
- Add logging when returning error in auth middleware (#1694)
- *(sync)* Allow to force a full sync anytime (#1658)

### Changed

- *(deps)* Bump undici from 6.2.1 to 6.6.1 (#1689)
- Remove unecessary call to API (#1709)
- Rate limiter v1 (#1708)
- Enable sdk telemetry (#1715)

### Fixed

- *(sync)* Always trust lastSyncDate (#1685)
- *(activity)* UI filters are inverted (#1688)
- *(datadog)* Incorrect metric for sync  (#1695)
- Error response logging (#1699)
- *(ui)* Track getting started (#1700)
- *(cron)* Delete old activities safely (#1698)
- *(dd)* Correctly load tracer (#1705)
- *(cron)* Fine tune delete old activities (#1706)
- *(cron)* Env naming (#1714)

## [v0.37.24] - 2024-02-16

### Added

- *(telemetry)* Use dd-trace for metrics (#1681)
- *(activity)* Connection and integration filters in activities (#1648)
- *(integrations)* Integration template for hibob (#1636)

### Fixed

- *(datadog)* Incorrect instrumentation (#1671)
- *(cli)* Remember upgrade choice (#1666)
- *(sdk)* Deprecate setLastSyncDate() (#1679)
- *(activity)* Limit the number of logs displayed (#1665)

## [v0.37.23] - 2024-02-14

### Added

- Add retry for greenhouse (#1660)

### Changed

- Dev clean up (#1651)
- Use hosted tag for nango-server (#1663)

### Fixed

- *(demo)* Run every 5minutes (#1649)
- *(demo)* Auto idle demo after a few days (#1631)
- *(docker)* Dist is not compiled in the docker image but copied (#1654)
- Wrong export (#1655)
- *(ui)* Autocomplete new password (#1652)
- ConnectionConfigParams parsing (#1659)
- *(jobs)* Missing package (#1661)
- *(ci)* Dedup jobs (#1653)
- *(ci)* Incorrect commit sha in PR (#1664)
- *(runner)* Proper typing  (#1634)
- *(ci)* Bad substition (#1667)
- *(ci)* Missing alternatives on master (#1668)
- Fix action guide link (#1669)

## [v0.37.22] - 2024-02-08

### Changed

- Proxy should log to console (#1640)
- Eslint upgrade (#1630)

## [v0.37.21] - 2024-02-08

### Changed

- Reduce js bundle size by a 1/3 with lazy routes (#1577)

### Fixed

- *(action)* Be stricter about error and activity log  (#1628)

## [v0.37.20] - 2024-02-07

### Added

- *(integrations)* Linear incoming webhooks support (#1617)

### Changed

- Eslint --fix (#1627)

### Fixed

- *(webhooks)* Select only configured syncs (#1621)

## [v0.37.19] - 2024-02-06

### Added

- *(reporting)* Add error in datadog APM (#1615)

### Fixed

- *(activity)* Reduce time and memory allocated for cleaning the table (#1616)

## [v0.37.17] - 2024-02-02

### Fixed

- Webapp version number flick (#1578)

## [v0.37.13] - 2024-02-02

### Changed

- Improve errors logging + lastSyncDate = new Date if undefined (#1586)
- Filter config param if in response_metadata (#1570)
- Increase request size limit (#1594)
- Always track records size/count, not just when writing was successful (#1596)

### Fixed

- Error detail for postgresql 22001 error (#1597)

## [v0.37.9] - 2024-01-30

### Fixed

- Update sync connection frequency tooling and documentation (#1549)
- Update frontend version in webapp package after publication (#1571)
- *(api)* Deploying sync now keeps frequency override (#1556)

## [v0.37.8] - 2024-01-26

### Changed

- Link account and environment to authenticated trace (#1564)

## [v0.37.7] - 2024-01-25

### Changed

- Explicitly install qs (#1565)

## [v0.37.5] - 2024-01-25

### Fixed

- *(ui)* Show frequency in connection's sync page (#1559)

## [v0.37.4] - 2024-01-24

### Added

- Override sync frequency  (#1548)

### Fixed

- Fix type of the updateMetadata function (#1557)
- *(api)* /sync/status returns execution frequency (#1550)

## [v0.37.2] - 2024-01-23

### Fixed

- *(dev)* Upgrade eslint minors (#1546)

## [v0.37.1] - 2024-01-22

### Added

- Adding logs to debug why Nango.auth() sometimes doesn't resolve (#1312)
- Add support for apollo.io (#1466)
- Add option to auth() to enable closed window detection (#1533)

### Changed

- Revert auth popup closing detection and race condition fix (#1310)
- Buffer should be available inside Node.vm (#1443)
- Fallback to default runner if account runner is not ready quickly (#1440)
- Caching runner (#1505)
- Disable login window detection when needed (#1528)

### Fixed

- Fix setMetadata argument type (#1428)
- NangoProps lastSyncDate is not decoded as a Date (#1451)
- Runner can run script for up to 24h (#1462)
- Fix no res response
- If condition in push container github action (#1504)
- Jobs should depends on shared v0.36.88 (#1512)

## [v0.36.14] - 2023-11-13

### Added

- Key rotation warning (#1196)

### Changed

- *(webapp)* Improve sidebar ui design (#1163)

## [v0.24.4] - 2023-07-13

### Added

- Add separate command to migrate database (#663)

### Changed

- Updated provider wiki. (#618)
- Improve explanation of nango.auth params in quickstart (#626)
- Segment to add basic authorization method (#604)
- Allow the websockets path to be configured (#688)

### Fixed

- Docker compose volumes on windows (#625)

## [v0.16.0] - 2023-05-02

### Added

- Add provider for Timely (#576)
- Force refresh token on the web UI (#587)
- *(server/db)* 💾 Add support for connection pool overrides (#588)
- Introduce hmac feature to restrict creation of new connections (#591)
- Query connections for only a specific connectionId. (#596)

### Fixed

- Input overlaps (#584)
- Correctly display error message when creating a connection (#589)
- Error messages when scopes are missing (#592)

## [v0.15.1] - 2023-04-24

### Added

- Adds Bamboo HR provider config. (#486)
- Hide secrets by default (#553)
- Custom error handler (#557)
- Added new scripts to gen source-maps on install (#542)
- Tags input for entering scopes (#556)
- Add copy option to secret button (#560)
- Added tiny space between nav items (#564)
- Prism component with super powers (#563)

### Changed

- Generic layouts for dashboard and default pages (#550)
- Render Default Scope from Providers. (#534)

### Fixed

- Make frontend sdk ssr friendly (#565)

## [v0.14.0] - 2023-04-18

### Added

- Added Provider for battlenet (#513)
- Deel Provider (#512)
- Add feature for Gorilla health (#497)
- Add provider for Accelo (#540)
- Add teamwork providers (#539)
- Added Provider for docusign (#533)
- Add providers for Uber. (#532)
- Add Bold sign provider. (#531)
- Add Provider for Squareup (#530)
- Add outreach provider (#529)
- Added Zoho-desk provider (#524)
- Added Provider for pandadoc. (#523)

### Changed

- Add a table to persist OAuth Session (#426)
- Add Provider for Keep (#522)

### Fixed

- Mural authorization URL. (#514)
- Fix typo (#526)

## [v0.13.4] - 2023-04-11

### Added

- Add Strava provider (#434)
- Atlassian Provider (#432)
- Add Spotify as a provider (#431)
- Add integration for Mural (#464)
- Add one drive provider. (#498)
- Add Amazon Provider (#496)
- Added oAuth for payfit (#485)
- Add provider for typeform (#484)
- Add provider for Gorgias (#483)

### Changed

- Added Twitch provider. (#435)
- Segment integration (#425)
- Added Yandex Provider. (#436)
- Add Mailchimp provider (#428)
- Add Figma Provider (#440)
- Added Provider for Figjam (#462)
- Add Zenefits Provider (#472)
- Add support for querying an immediate refresh of the provider's refresh token (#465)
- Adobe Service integration (#463)
- Add provider for Gusto. (#473)
- Connection config params (#474)
- Fixes #386 by changing the UI routes for the 'connections' pages (#478)

### Fixed

- Bad request request when requesting for refresh token (#430)
- Asana Integrations (#456)
- Added Provider for Miro. (#457)
- Digital Ocean refresh token (#500)
- Allow use of dynamic port for Nango DB in docker compose. (#499)
- Connection create page. (#489)

## [v0.12.7] - 2023-03-31

### Added

- Added precommit hook (#396)

### Fixed

- *(app)* Encode URLs when redirecting (#424)
- Refresh token contenstack integrations (#398)

## [v0.12.1] - 2023-03-24

### Added

- Added server version on startup logs. (#380)

### Changed

- 🎡 add nodemon for development (#381)

## [v0.11.2] - 2023-03-21

### Added

- Dashboard: Confirmation before delete (#373)

### Changed

- ⚡️ added docker volume to the postgres in docker-compose (#376)

## [v0.8.5] - 2023-02-17

### Changed

- Support one-click deployment for render & heroku (#329)

## [v0.8.0] - 2023-02-13

### Changed

- Add a one-click deploy to render button (#317)

## [v0.5.1] - 2023-01-17

### Added

- Add support for Brex

## [v0.3.6] - 2022-11-30

### Changed

- Rewrite (details in desc)

## [v0.2.2] - 2021-06-08

### Added

- Add automation to publish container image (#227)

## [v0.2.1] - 2021-05-12

### Added

- Add env.example
- Build with webpack
- Add postgresql
- Add knex
- Add procfile
- Add ts node for deployment
- Persist session
- Add more logging
- Add authentications
- Store result from authentication
- Add authId
- Add save-setup and retrieve-setup
- Add timestamps to configurations
- Add setupId
- Allow user to provide it's own callback url
- Prepare README structure
- Add dashboard views
- Passing API config to frontend
- Link users view to database
- Link dashboard to database
- Add images to the integrations - WIP using Clearbit
- Handle errors on the dashboard
- Api endpoints
- Add deletion actions on the dashboard
- Updating JS client to Pizzly
- Adding first batch of tests
- Add integration methods
- Handle proxy requests
- Update Pizzly's main config files
- Improve common page (home, errors, etc.)
- Click&go connect button
- Introduce a 'prepare' script
- Secure access to the dashboard
- Improve how the errors from the API are returned
- Secure access to the API using a secret key
- Improve API errors on unauthenticated requests
- Proxy feature unauthentificated requests
- Support of proxy requests for OAuth2
- Handle passing body content in the proxy request
- Secure access to auth and proxy
- New route on the API to retrieve an integration's config
- Handle errors on the API with PizzlyError
- Option to limit frontend call to the proxy service
- Save setup id with a successful authentication
- Add publishable key to pizzly js
- Publish pizzly js
- Update version with request authentication
- Review README
- Review images
- Handle summary
- Add license
- Update images
- Update images
- Reduce logo width
- Handle supported APIs
- Handle token refreshness for OAuth2
- Add favicon (#33)
- Support of Pizzly initialization with a string (#36)
- Reduce the amount of environment for Heroku (#39)
- Add dev command
- Add logger
- Add option to enable Bearer.sh (#44)
- Add views directory to the docker image (#61)
- Added integration file for google hangouts (#152)
- New pizzly-js release
- Drift.com-integration (#155) (#163)
- Add HSTS header (#159)
- Enable telemetry data (#169)
- Prepare product hunt (#170)
- Add a try this authId link (#171)
- Improve error message on token refreshness (#176)

### Changed

- Update dependencies
- Dev commands
- Get rid of webpack for server
- Move integrations out of src
- Knex migrations
- Disable migration temporarily
- Re enable migrations
- Enless command
- Providfe mode
- Use correct location
- Clean up
- Removing some old code
- Remove ts-node dependency
- Split api/dashboard/auth/proxy into differents routers
- Clean routes accross each feature
- Group all things DB in this file
- Moved src/views to views/
- Uses ejs as template engine
- Remove tslint for now
- Cleanup exressp's app generator
- Nasty credentials
- Moved clients/ under the auth/ directory
- Review JS client README
- Migrate some views
- Remove logs
- Cleanup following updates to the JS client
- Moving auth directory to new legacy dir
- Moving functions dir to new legacy dir
- Moving middleware dir to new legacy dir
- Moving api-config dir to new legacy dir
- Moving functions dir to new legacy dir
- Revert change to test the connect
- Ease onboarding with low config
- Migration of user_attributes to payload
- Migration of clientID to clientId
- Migration of config.setup to config.credentials
- Moved error-handler to legacy directory
- How we handle global errors
- Reduce global middlewares
- Improve comments on the access library
- Remove API reference from README, now in the wiki
- Rename credentials to configurations
- Use of configurations where appropriate
- Rename dashboard user/password
- Upgrade typescript and fix tests
- : use pipe whenever it is possible
- Update link
- *(deps)* Bump lodash in /src/clients/javascript (#81)
- *(deps)* Bump lodash from 4.17.15 to 4.17.19 in /src/clients/node (#82)
- Pull-request template
- Pull-request template in the right directory
- *(deps)* Bump node-fetch from 2.6.0 to 2.6.1 in /src/clients/node (#94)
- *(deps-dev)* Bump node-fetch from 2.6.0 to 2.6.1 (#95)
- Link to demo app
- Update PR template (#160)
- Adding Monday.com integration (#167)
- Adding fitbit.com integration (#172)
- Splitwise integration (#188)
- Invalid Google cloud URL (#202)

### Fixed

- Remove legacy files
- Build server
- Remvoe legacy references
- Fix render enndine
- Views path
- Bring back auth id
- Fix app.json
- Use config foler
- Fix dependencies
- Test unsecure
- Set secure to true
- SaveUnitialized
- Use ejs instead of mustache
- Get rid of aliasBuid
- Include json files
- Trigger build
- Log getAuth
- Clean up
- Reduce pool setup
- Update pool config for db
- Share connections
- Trigger build
- Fix fetchAuthDetails
- Reuse db connection
- Fix validator
- Fix scopes
- Fix tests
- Update slack scope
- Fix setupId
- Fix setupdetails
- Fix oauth2
- Fix storage
- Fix migrations
- Fix migration
- Update URL with new Pizzly repo
- Use of legacy proxy code to provide proxy endpoint (for now)
- Set logo dimensions
- Using cp temporary to copy more views
- Removing vhost - we don't use it anymore
- Use new callback URl per default
- Plus icon to add an API
- Some issue following migration
- Remove Axios from type definition
- Handle edge case with the auth process
- Issue with credentials rendering
- Auth by forcing a callbackUrl
- UX fixes
- Handle unauthorized errors (401)
- Remove access management on /auth
- Update README
- Minimize summary
- Minimize summary
- Try to use local images
- Minor typo
- A few more relative links
- Headings
- Finish renaming of .credential to .configuration (#32)
- Issue when the setupId is unknown (#34)
- Issue with setupId
- Support multiple scopes (one per line) (#42)
- Fix test config
- Remove Bearer's callback URL (#46)
- Enable cors on proxy (#48)
- No-default scope on integrations (#49)
- Hotfix on configuration auth properties
- Hotfix on req.data.integration renaming
- Typos (#54)
- Open port locally
- Force publish change to pizzly-js
- Remove project link + version (#149)
- Handle param options (#154)
- Update Zendesk Chat configuration file (#161)
- APIs using client_credentials as grant type (#165)

[0.39.28]: https://github.com/NangoHQ/nango/compare/v0.39.27..0.39.28
[v0.39.27]: https://github.com/NangoHQ/nango/compare/v0.39.26..v0.39.27
[v0.39.26]: https://github.com/NangoHQ/nango/compare/v0.39.25..v0.39.26
[v0.39.25]: https://github.com/NangoHQ/nango/compare/v0.39.24..v0.39.25
[v0.39.24]: https://github.com/NangoHQ/nango/compare/v0.39.23..v0.39.24
[v0.39.23]: https://github.com/NangoHQ/nango/compare/v0.39.22..v0.39.23
[v0.39.22]: https://github.com/NangoHQ/nango/compare/v0.39.21..v0.39.22
[v0.39.21]: https://github.com/NangoHQ/nango/compare/v0.39.20..v0.39.21
[v0.39.20]: https://github.com/NangoHQ/nango/compare/v0.39.19..v0.39.20
[v0.39.19]: https://github.com/NangoHQ/nango/compare/v0.39.18..v0.39.19
[v0.39.18]: https://github.com/NangoHQ/nango/compare/v0.39.17..v0.39.18
[v0.39.17]: https://github.com/NangoHQ/nango/compare/v0.39.16..v0.39.17
[v0.39.16]: https://github.com/NangoHQ/nango/compare/v0.39.15..v0.39.16
[v0.39.14]: https://github.com/NangoHQ/nango/compare/v0.39.13..v0.39.14
[v0.39.13]: https://github.com/NangoHQ/nango/compare/v0.37.0..v0.39.13
[v0.37.0]: https://github.com/NangoHQ/nango/compare/v0.39.8..v0.37.0
[v0.39.8]: https://github.com/NangoHQ/nango/compare/v0.39.7..v0.39.8
[v0.39.7]: https://github.com/NangoHQ/nango/compare/v0.39.6..v0.39.7
[v0.39.6]: https://github.com/NangoHQ/nango/compare/v0.39.5..v0.39.6
[v0.39.5]: https://github.com/NangoHQ/nango/compare/v0.39.4..v0.39.5
[v0.39.4]: https://github.com/NangoHQ/nango/compare/v0.39.3..v0.39.4
[v0.39.3]: https://github.com/NangoHQ/nango/compare/v0.39.2..v0.39.3
[v0.39.2]: https://github.com/NangoHQ/nango/compare/v0.39.1..v0.39.2
[v0.39.1]: https://github.com/NangoHQ/nango/compare/v0.39.0..v0.39.1
[v0.39.0]: https://github.com/NangoHQ/nango/compare/v0.38.5..v0.39.0
[v0.38.5]: https://github.com/NangoHQ/nango/compare/v0.38.4..v0.38.5
[v0.38.4]: https://github.com/NangoHQ/nango/compare/v0.38.3..v0.38.4
[v0.38.3]: https://github.com/NangoHQ/nango/compare/v0.38.2..v0.38.3
[v0.38.2]: https://github.com/NangoHQ/nango/compare/v0.38.1..v0.38.2
[v0.38.1]: https://github.com/NangoHQ/nango/compare/v0.38.0..v0.38.1
[v0.38.0]: https://github.com/NangoHQ/nango/compare/v0.37.26..v0.38.0
[v0.37.26]: https://github.com/NangoHQ/nango/compare/v0.37.25..v0.37.26
[v0.37.25]: https://github.com/NangoHQ/nango/compare/v0.37.24..v0.37.25
[v0.37.24]: https://github.com/NangoHQ/nango/compare/v0.37.23..v0.37.24
[v0.37.23]: https://github.com/NangoHQ/nango/compare/v0.37.22..v0.37.23
[v0.37.22]: https://github.com/NangoHQ/nango/compare/v0.37.21..v0.37.22
[v0.37.21]: https://github.com/NangoHQ/nango/compare/v0.37.20..v0.37.21
[v0.37.20]: https://github.com/NangoHQ/nango/compare/v0.37.19..v0.37.20
[v0.37.19]: https://github.com/NangoHQ/nango/compare/v0.37.18..v0.37.19
[v0.37.17]: https://github.com/NangoHQ/nango/compare/v0.37.16..v0.37.17
[v0.37.13]: https://github.com/NangoHQ/nango/compare/v0.37.12..v0.37.13
[v0.37.9]: https://github.com/NangoHQ/nango/compare/v0.37.8..v0.37.9
[v0.37.8]: https://github.com/NangoHQ/nango/compare/v0.37.7..v0.37.8
[v0.37.7]: https://github.com/NangoHQ/nango/compare/v0.37.6..v0.37.7
[v0.37.5]: https://github.com/NangoHQ/nango/compare/v0.37.4..v0.37.5
[v0.37.4]: https://github.com/NangoHQ/nango/compare/v0.37.3..v0.37.4
[v0.37.2]: https://github.com/NangoHQ/nango/compare/v0.37.1..v0.37.2
[v0.37.1]: https://github.com/NangoHQ/nango/compare/v0.36.14..v0.37.1
[v0.36.14]: https://github.com/NangoHQ/nango/compare/v0.35.5..v0.36.14
[v0.24.4]: https://github.com/NangoHQ/nango/compare/v0.16.0..v0.24.4
[v0.16.0]: https://github.com/NangoHQ/nango/compare/v0.15.1..v0.16.0
[v0.15.1]: https://github.com/NangoHQ/nango/compare/v0.14.0..v0.15.1
[v0.14.0]: https://github.com/NangoHQ/nango/compare/v0.13.5..v0.14.0
[v0.13.4]: https://github.com/NangoHQ/nango/compare/v0.12.7..v0.13.4
[v0.12.7]: https://github.com/NangoHQ/nango/compare/v0.12.6..v0.12.7
[v0.12.1]: https://github.com/NangoHQ/nango/compare/v0.11.3..v0.12.1
[v0.11.2]: https://github.com/NangoHQ/nango/compare/v0.10.7..v0.11.2
[v0.8.5]: https://github.com/NangoHQ/nango/compare/v0.8.0..v0.8.5
[v0.8.0]: https://github.com/NangoHQ/nango/compare/v0.7.2..v0.8.0
[v0.5.1]: https://github.com/NangoHQ/nango/compare/v0.5.0..v0.5.1
[v0.3.6]: https://github.com/NangoHQ/nango/compare/v0.2.2..v0.3.6
[v0.2.2]: https://github.com/NangoHQ/nango/compare/v0.2.1..v0.2.2

<!-- generated by git-cliff -->
