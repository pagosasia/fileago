v1.5.0 - 10 Apr 2020
---

* Chat and video integration with Rocket.chat
* Disable printing from browser on public shares
* Accomodate incorrect urls in webdrive endpoint for broken clients
* Add FileAgo version and license API endpoints
* Allow updating license from Admin Panel
* Minor UI enhancements and bugs also fixed

v1.4.1 - 18 Feb 2020
---

* Password protected public shares implementation
* Fixed bug of files reporting incorrect updated time
* Major architecture improvements in WebDrive
* All deleted file revisions are now cleaned up from database
* Maximum number of revisions now limited to 500
* Maximum number of revisions for .slog and .dat files via WebDrive limited to 10
* "Private share create" permission logic applies for copy sharing too
* New config option in internal db: "allow_sharing_with_all_groups"
* Ldap group sync functionality implementation
* Ldap attribute "faDefaultQuota" to override quota value for individual users and groups
* Support to skip WebDrive LOCK checks internally if needed
* "If-None-Match" header support for WebDrive urls
* Fixed bug where WebDrive was listing blocked resources
* WebDrive replies now has cache-control header set to 'no-cache'
* Fixed issues when file end up with multiple revisions having same timestamp
* Some other minor bugs fixed

v1.4.0 - 8 Dec 2019
---

* FileAgo WebDrive (WebDAV) implementation
* Encrypt and Preview manager processes now use different sqlite dbs
* Send custom message in email while creating pubic shares
* Support for usage of 'latest' and 'oldest' in file download url
* File downloads reply now have Content-Length header set
* Various other minor bugs fixed

v1.3.1 - 24 Sep 2019
---

* Fixed bug where chunk creation failed for empty files
* Notification emails now use images hosted at fileago.com
* Fixed bug where API auth was crashing sometimes due to exceptions
* Notification emails now more compatible to email standards

v1.3.0 - 6 Aug 2019
---

* Variable size file chunking algorithm support
* Fixed bug regarding public share emails not getting sent
* Creating new dir returns http 200 with data now, and not 204
* ldapsearch can now do paged searches and fetch all results
* Removed websocket connect/disconnect popup notification
* Fixed bug where files created via WOPI was not respecting disk quota restrictions
* Added support for preview of CAD files
* Added support for sync agent application
* Many minor bugs also fixed

v1.2.0 - 11 Mar 2019
---

* Added '15 days' as an option to keep file old revisions
* Added support for Factor Authentication (TOTP based)
* Added support for LDAP/AD authentication
* Download is a new permission option (along with existing r,w,d)
* Public shares also need download permission for file downloads
* FileAgo can now function as a WOPI host
* Completed integration with LibreOffice Online
* Switched from Neo4j to latest OngDB database

v1.1.0 - 30 Nov 2018
---

* Added OPTIONS for /auth endpoint
* Added OPTIONS for /upload/:token endpoint
* Added OPTIONS for /resources/auth/* urls
* Added support for AES-256-GCM encryption of uploaded files
* Fixed many critical bugs related to permissions and user access

v1.0.0 - 23 Oct 2018
---

* First release
