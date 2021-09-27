<div align="center">
  <h1><img alt="Logo" src="https://raw.githubusercontent.com/tropicalraisel/skylib/master/.github/images/logo.svg" width="300">/ skylib</h1>
  <p>Skypack for all!</p>
  <hr>
  <p>Check out Skypack's <a href="https://docs.skypack.dev/#whats-old-is-new-again">official documentation</a>!</p>
  <hr>
  <p>
    <a href="https://www.npmjs.com/package/@tropicalraisel/skylib">
      <img alt="npm" src="https://img.shields.io/npm/v/@tropicalraisel/skylib?style=flat&logo=npm&label=npm&color=CB3837">
    </a>
    <a href="https://github.com/google/gts">
      <img alt="Google Badge" src="https://img.shields.io/static/v1?style=flat&logo=google&label=google&message=code%20style&color=4285F4">
    </a>
    <a href="https://www.npmjs.com/package/@tropicalraisel/skylib">
      <img alt="npms.io" src="https://img.shields.io/npms-io/quality-score/@tropicalraisel/skylib?style=flat">
    </a>
    <a href="https://david-dm.org/tropicalraisel/skylib">
      <img alt="daviddm" src="https://status.david-dm.org/gh/tropicalraisel/skylib.svg">
    </a>
    <a href="https://david-dm.org/tropicalraisel/skylib?type=dev">
      <img alt="daviddm-dev" src="https://status.david-dm.org/gh/tropicalraisel/skylib.svg?type=dev">
    </a>
  </p>
</div>

## API

`SKYPACK_URL: string`: Equals the following: https://cdn.skypack.dev

`isValidVersion(package_version: string): boolean`: Returns if Skypack will accept the passed package version.

`isValidPackage(package_id: string): boolean`: Returns if Skypack will accept the passed package ID.

`getSkypackUrl(package_id: string, minified = true): Promise<string>`: Returns the most optimal Skypack URL for a passed package ID, which is usually a [pinned URL](https://docs.skypack.dev/skypack-cdn/api-reference/pinned-urls-optimized). If the package ID is invalid, it will be returned.
