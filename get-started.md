# Getting started with our bug bounty program

* **Grafana OSS** - we offer Docker images that are synced with the `main` branch. This makes it easy to get started right away and be sure that you're looking for issues in an untouched instance. To spin up Grafana OSS in Docker, run the following command:

    `docker run -p 3000:3000 grafana/grafana-oss:main` and then visit http://localhost:3000 and login with `admin:admin`

You can also follow this [guide](https://grafana.com/docs/grafana/latest/setup-grafana/installation/docker/) on how to run the Grafana Docker image.

* **Mimir** - you can get started by following [Get started with Grafana Mimir](https://grafana.com/docs/mimir/latest/get-started/).

## Understanding the threat model for Grafana

Please refer to the following [documentation page](https://grafana.com/docs/grafana/latest/administration/roles-and-permissions/) in order to understand the roles and permissions in Grafana.

Non-core plugins are considered out of scope as Grafana administrators install them at their own risk. 

## Accepted risks
* **Grafana**: A user with Viewer role that can tamper with dashboard queries [[documentation](https://grafana.com/docs/grafana/latest/setup-grafana/configure-security/#limit-viewer-query-permissions)]
* **Grafana**: Exposed JWT tokens in URL's when url_login is enabled [[issue](https://github.com/grafana/bugbounty/security/advisories/GHSA-5585-m9r5-p86j)]
* **Grafana**: Data sources that have been deliberately manipulated to exploit a weakness in Grafana [[issue](https://github.com/grafana/bugbounty/security/advisories/GHSA-qrrg-gw7w-vp76)]
* **Mimir**: CSRF issues [[issue](https://github.com/grafana/bugbounty/security/advisories/GHSA-2wxq-mcch-gvxv)]

## Issues of particular interest
* Authentication issues.
* Cross-Site-Scripting, DOM clobbering, prototype pollution and other client side issues.
* For previously found vulnerabilities, see: https://grafana.com/security/security-advisories/
