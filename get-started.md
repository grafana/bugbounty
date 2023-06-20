# How to get started in the Grafana Labs bug bounty program

* **Grafana OSS** - we offer docker images that are synced with the `main` branch. This makes it easy to get started right away and be sure that you're looking for issues in an untouched instance. To spin up Grafana OSS in docker, run the following command:

    `docker run -p 3000:3000 grafana/grafana-oss:main` and then visit http://localhost:3000 and login with `admin:admin`

* **Mimir** - you can get started by following [Play with Grafana Mimir](https://grafana.com/tutorials/play-with-grafana-mimir/).

## Understanding the threat model for Grafana

Please refer to the following [documentation page](https://grafana.com/docs/grafana/latest/administration/roles-and-permissions/) in order to understand the roles and permissions in Grafana.

Installed non-core plugins are considered to be trusted so any vulnerability affecting those will be handled outside of the bug bounty program. 

## Accepted risks
* **Grafana**: A user with Viewer role that can tamper with dashboard queries [[documentation](https://grafana.com/docs/grafana/latest/setup-grafana/configure-security/#limit-viewer-query-permissions)]
* **Grafana**: Exposed JWT tokens in URL's when url_login is enabled [[issue](https://github.com/grafana/bugbounty/security/advisories/GHSA-5585-m9r5-p86j)]
* **Grafana**: Data sources that have been deliberately manipulated to exploit a weakness in Grafana [[issue](https://github.com/grafana/bugbounty/security/advisories/GHSA-qrrg-gw7w-vp76)]
* **Mimir**: CSRF issues [[issue](https://github.com/grafana/bugbounty/security/advisories/GHSA-2wxq-mcch-gvxv)]

## Issues that we are particular interested in
* Authentication issues.
* Cross-Site-Scripting, DOM clobbering, prototype pollution and other client side issues.
