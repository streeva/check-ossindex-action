# Check OSS Index
GitHub Action that checks a list of dependencies against the Sonatype OSS Index

This tool is designed to work against the CSV file that is output by [streeva/read-dependencies-go](https://github.com/streeva/read-dependencies-go) or [streeva/read-dependencies-action](https://github.com/streeva/read-dependencies-action)

The application will attempt to post message(s) about any vulnerabilities found to Slack via a custom bot if you set-up a custom app and provide a Bot User OAuth Access Token.

Checks will be made against the OSS Index anonymously by default, but they are rate-limited, if you find you are getting told to back off by the service you can [sign-up for free](https://ossindex.sonatype.org/user/register) and this gives you an increase to the access limit.

# Usage

See [action.yml](action.yml)