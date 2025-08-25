# 26319
Reproduction for [Renovate discussion 26319](https://github.com/renovatebot/renovate/discussions/26319).

## Current behavior

Renovate fails to look up the Dart git package.
<img width="1288" height="352" alt="image" src="https://github.com/user-attachments/assets/519ff3a3-b094-4cf3-91e4-adac220517f4" />
It appears to try to find it on `pub.dev`:

`DEBUG: GET https://pub.dartlang.org/api/packages/example_git_package = (code=ERR_NON_2XX_3XX_RESPONSE, statusCode=404 retryCount=0, duration=264)`

## Expected behavior

Renovate should successfully look up the dependency using the URL from the pubspec.

## Link to the Renovate issue or Discussion

https://github.com/renovatebot/renovate/discussions/26319
