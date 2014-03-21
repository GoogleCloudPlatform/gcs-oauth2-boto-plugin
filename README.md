# gcs-oauth2-boto-plugin

gcs-oauth2-boto-plugin is a Python application whose purpose is to behave as
an auth plugin for the boto[1] auth plugin framework for use with OAuth 2.0
credentials[2] for the Google Cloud Platform. This plugin is compatible with
both user accounts[3] and service accounts[4], and its functionality is
essentially a wrapper around the oauth2client package of
google-api-python-client[5] with the addition of automatically caching tokens
for the machine in a thread- and process-safe fashion.

For more information about how to use this plugin to access Google Cloud Storage
via boto in your application, see the GCS documentation[6].

Before submitting any code, please run the tests (e.g., by running the following
command from the root of this repository):
  python oauth2_plugin/test_oauth2_client.py

[1]: https://github.com/boto/boto
[2]: https://developers.google.com/accounts/docs/OAuth2Login
[3]: https://developers.google.com/accounts/docs/OAuth2#installed
[4]: https://developers.google.com/accounts/docs/OAuth2#serviceaccount
[5]: https://code.google.com/p/google-api-python-client/wiki/OAuth2Client
[6]: https://developers.google.com/storage/docs/gspythonlibrary
