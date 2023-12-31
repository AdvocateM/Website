# Exporting

Users can export their media history using the `/export` endpoint. We do not have
a custom interface to perform exports, so you will have to do some steps manually.

1. Login to your Ryot instance and copy your auth cookie.

	![Auth cookie](/docs/assets/auth-cookie.png)

2. Execute the following curl command:

  ```bash
  curl <ryot_url>/export --header 'Authorization: Bearer <auth_cookie>'
  ```

  For example:

  ```bash
  curl 'https://ryot.fly.dev/export' --header 'Authorization: Bearer 0ab88f6b-768a-4d65-885b-502016b634e0'
  ```